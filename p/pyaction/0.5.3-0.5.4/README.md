# Comparing `tmp/pyaction-0.5.3.tar.gz` & `tmp/pyaction-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaction-0.5.3.tar", last modified: Sat Apr 13 14:31:33 2024, max compression
+gzip compressed data, was "pyaction-0.5.4.tar", last modified: Mon Apr 15 06:32:23 2024, max compression
```

## Comparing `pyaction-0.5.3.tar` & `pyaction-0.5.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:31:33.608481 pyaction-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-13 14:31:29.000000 pyaction-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 14:31:29.000000 pyaction-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-13 14:31:33.608481 pyaction-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-13 14:31:29.000000 pyaction-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:31:33.604480 pyaction-0.5.3/pyaction/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:31:33.608481 pyaction-0.5.3/pyaction/issues/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/issues/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/issues/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:31:33.608481 pyaction-0.5.3/pyaction/template/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/template/copier.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:31:33.608481 pyaction-0.5.3/pyaction/template/{{action_slug}}/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/template/{{action_slug}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/template/{{action_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/template/{{action_slug}}/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/template/{{action_slug}}/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/template/{{action_slug}}/action.yml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/template/{{action_slug}}/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/template/{{action_slug}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:31:33.604480 pyaction-0.5.3/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:31:33.608481 pyaction-0.5.3/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:31:33.608481 pyaction-0.5.3/pyaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-13 14:31:33.000000 pyaction-0.5.3/pyaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-13 14:31:33.000000 pyaction-0.5.3/pyaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:31:33.000000 pyaction-0.5.3/pyaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 14:31:33.000000 pyaction-0.5.3/pyaction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-13 14:31:33.000000 pyaction-0.5.3/pyaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 14:31:33.000000 pyaction-0.5.3/pyaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-13 14:31:29.000000 pyaction-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:31:33.608481 pyaction-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 06:32:18.000000 pyaction-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 06:32:18.000000 pyaction-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-15 06:32:23.023181 pyaction-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-15 06:32:18.000000 pyaction-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.019181 pyaction-0.5.4/pyaction/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/issues/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/issues/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/copier.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction/template/{{action_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/action.yml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.019181 pyaction-0.5.4/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:32:23.023181 pyaction-0.5.4/pyaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 06:32:23.000000 pyaction-0.5.4/pyaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-15 06:32:18.000000 pyaction-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 06:32:23.023181 pyaction-0.5.4/setup.cfg
```

### Comparing `pyaction-0.5.3/LICENSE` & `pyaction-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.3/PKG-INFO` & `pyaction-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.3
+Version: 0.5.4
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyaction-0.5.3/README.md` & `pyaction-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.3/pyaction/cli.py` & `pyaction-0.5.4/pyaction/cli.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.3/pyaction/io.py` & `pyaction-0.5.4/pyaction/io.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.3/pyaction/issues/connector.py` & `pyaction-0.5.4/pyaction/issues/connector.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.3/pyaction/template/copier.yml` & `pyaction-0.5.4/pyaction/template/copier.yml`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.3/pyaction.egg-info/PKG-INFO` & `pyaction-0.5.4/pyaction.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.3
+Version: 0.5.4
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyaction-0.5.3/pyaction.egg-info/SOURCES.txt` & `pyaction-0.5.4/pyaction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.3/pyproject.toml` & `pyaction-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaction"
-version = "0.5.3"
+version = "0.5.4"
 description = "Create GitHub Actions using Python"
 authors = [{ name = "Sadra Yahyapour", email = "lnxpylnxpy@gmail.com" }]
 requires-python = ">=3.8"
 dependencies = [
     "copier >= 9.2",
     "click >= 8.1",
     "pygithub >= 2.3.0",
@@ -25,16 +25,19 @@
 docs = ["mkdocs-material", "cairosvg", "pillow"]
 
 [project.urls]
 Documentation = "https://pyaction.imsadra.me"
 Repository = "https://github.com/lnxpy/pyaction"
 
 [tool.bumpversion]
-current_version = "0.5.3"
+current_version = "0.5.4"
 commit = "true"
 tag = "true"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 
 [[tool.bumpversion.files]]
 filename = "pyaction/__init__.py"
+
+[[tool.bumpversion.files]]
+filename = "pyaction/template/{{action_slug}}/requirements.txt"
```

