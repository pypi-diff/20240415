# Comparing `tmp/aixblock_ml-0.0.5.tar.gz` & `tmp/aixblock_ml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_ml-0.0.5.tar", max compression
+gzip compressed data, was "aixblock_ml-0.0.6.tar", max compression
```

## Comparing `aixblock_ml-0.0.5.tar` & `aixblock_ml-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       11 2024-04-03 07:28:40.006140 aixblock_ml-0.0.5/README.md
--rw-r--r--   0        0        0       84 2024-04-04 08:01:18.783734 aixblock_ml-0.0.5/aixblock_ml/__init__.py
--rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.0.5/aixblock_ml/api.py
--rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.5/aixblock_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.0.5/aixblock_ml/default_configs/README.md
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.490661 aixblock_ml-0.0.5/aixblock_ml/default_configs/_wsgi.py
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.0.5/aixblock_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.0.5/aixblock_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0     2129 2024-04-15 02:26:57.535807 aixblock_ml-0.0.5/aixblock_ml/default_configs/model.py
--rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.5/aixblock_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.5/aixblock_ml/exceptions.py
--rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.5/aixblock_ml/helpers.py
--rw-r--r--   0        0        0    35732 2024-04-15 02:32:53.891767 aixblock_ml-0.0.5/aixblock_ml/model.py
--rw-r--r--   0        0        0     7477 2024-04-15 02:26:57.534982 aixblock_ml-0.0.5/aixblock_ml/server.py
--rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.5/aixblock_ml/templates/preview.html
--rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.0.5/aixblock_ml/utils.py
--rw-r--r--   0        0        0      314 2024-04-15 02:46:13.033061 aixblock_ml-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 aixblock_ml-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-04-15 02:52:58.946494 aixblock_ml-0.0.6/README.md
+-rw-r--r--   0        0        0       84 2024-04-04 08:01:18.783734 aixblock_ml-0.0.6/aixblock_ml/__init__.py
+-rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.0.6/aixblock_ml/api.py
+-rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.6/aixblock_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.0.6/aixblock_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.490661 aixblock_ml-0.0.6/aixblock_ml/default_configs/_wsgi.py
+-rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.0.6/aixblock_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.0.6/aixblock_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0     2129 2024-04-15 02:26:57.535807 aixblock_ml-0.0.6/aixblock_ml/default_configs/model.py
+-rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.6/aixblock_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.6/aixblock_ml/exceptions.py
+-rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.6/aixblock_ml/helpers.py
+-rw-r--r--   0        0        0    35732 2024-04-15 02:32:53.891767 aixblock_ml-0.0.6/aixblock_ml/model.py
+-rw-r--r--   0        0        0     7477 2024-04-15 02:26:57.534982 aixblock_ml-0.0.6/aixblock_ml/server.py
+-rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.6/aixblock_ml/templates/preview.html
+-rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.0.6/aixblock_ml/utils.py
+-rw-r--r--   0        0        0      403 2024-04-15 06:36:52.267685 aixblock_ml-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 aixblock_ml-0.0.6/PKG-INFO
```

### Comparing `aixblock_ml-0.0.5/aixblock_ml/api.py` & `aixblock_ml-0.0.6/aixblock_ml/api.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/default_configs/README.md` & `aixblock_ml-0.0.6/aixblock_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/default_configs/_wsgi.py` & `aixblock_ml-0.0.6/aixblock_ml/default_configs/_wsgi.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/default_configs/_wsgi.py.tmpl` & `aixblock_ml-0.0.6/aixblock_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/default_configs/docker-compose.yml` & `aixblock_ml-0.0.6/aixblock_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/default_configs/model.py` & `aixblock_ml-0.0.6/aixblock_ml/default_configs/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/exceptions.py` & `aixblock_ml-0.0.6/aixblock_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/helpers.py` & `aixblock_ml-0.0.6/aixblock_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/model.py` & `aixblock_ml-0.0.6/aixblock_ml/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/server.py` & `aixblock_ml-0.0.6/aixblock_ml/server.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.5/aixblock_ml/utils.py` & `aixblock_ml-0.0.6/aixblock_ml/utils.py`

 * *Files identical despite different names*

