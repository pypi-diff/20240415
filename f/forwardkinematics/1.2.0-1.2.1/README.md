# Comparing `tmp/forwardkinematics-1.2.0.tar.gz` & `tmp/forwardkinematics-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forwardkinematics-1.2.0.tar", max compression
+gzip compressed data, was "forwardkinematics-1.2.1.tar", max compression
```

## Comparing `forwardkinematics-1.2.0.tar` & `forwardkinematics-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      582 2023-12-01 00:43:20.630890 forwardkinematics-1.2.0/README.md
--rw-r--r--   0        0        0      140 2023-12-01 00:43:36.730982 forwardkinematics-1.2.0/forwardkinematics/__init__.py
--rw-r--r--   0        0        0      330 2023-12-01 00:43:36.730982 forwardkinematics-1.2.0/forwardkinematics/fksCommon/fk.py
--rw-r--r--   0        0        0     2344 2023-12-01 00:43:36.730982 forwardkinematics-1.2.0/forwardkinematics/planarFks/planarArmFk.py
--rw-r--r--   0        0        0      677 2023-12-01 00:43:36.730982 forwardkinematics-1.2.0/forwardkinematics/planarFks/planar_fk.py
--rw-r--r--   0        0        0        0 2023-12-01 00:43:20.634890 forwardkinematics-1.2.0/forwardkinematics/urdfFks/casadiConversion/__init__.py
--rw-r--r--   0        0        0        0 2023-12-01 00:43:20.634890 forwardkinematics-1.2.0/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
--rw-r--r--   0        0        0     3442 2023-12-01 00:43:20.634890 forwardkinematics-1.2.0/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
--rw-r--r--   0        0        0     6240 2023-12-01 00:43:36.730982 forwardkinematics-1.2.0/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
--rw-r--r--   0        0        0      122 2023-12-01 00:43:36.730982 forwardkinematics-1.2.0/forwardkinematics/urdfFks/generic_urdf_fk.py
--rw-r--r--   0        0        0     4151 2023-12-01 00:43:36.730982 forwardkinematics-1.2.0/forwardkinematics/urdfFks/urdfFk.py
--rw-r--r--   0        0        0      715 2023-12-01 00:43:36.730982 forwardkinematics-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 forwardkinematics-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      582 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/README.md
+-rw-r--r--   0        0        0      205 2024-04-15 13:04:03.309632 forwardkinematics-1.2.1/forwardkinematics/__init__.py
+-rw-r--r--   0        0        0      330 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/fksCommon/fk.py
+-rw-r--r--   0        0        0     2344 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/planarFks/planarArmFk.py
+-rw-r--r--   0        0        0      677 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/planarFks/planar_fk.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
+-rw-r--r--   0        0        0     3442 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
+-rw-r--r--   0        0        0     6240 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
+-rw-r--r--   0        0        0      122 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/generic_urdf_fk.py
+-rw-r--r--   0        0        0     4151 2024-04-15 13:03:46.485598 forwardkinematics-1.2.1/forwardkinematics/urdfFks/urdfFk.py
+-rw-r--r--   0        0        0     7616 2024-04-15 13:04:03.309632 forwardkinematics-1.2.1/forwardkinematics/xmlFks/generic_xml_fk.py
+-rw-r--r--   0        0        0      762 2024-04-15 13:04:03.309632 forwardkinematics-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 forwardkinematics-1.2.1/PKG-INFO
```

### Comparing `forwardkinematics-1.2.0/README.md` & `forwardkinematics-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.0/forwardkinematics/planarFks/planarArmFk.py` & `forwardkinematics-1.2.1/forwardkinematics/planarFks/planarArmFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.0/forwardkinematics/planarFks/planar_fk.py` & `forwardkinematics-1.2.1/forwardkinematics/planarFks/planar_fk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.0/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py` & `forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.0/forwardkinematics/urdfFks/casadiConversion/urdfparser.py` & `forwardkinematics-1.2.1/forwardkinematics/urdfFks/casadiConversion/urdfparser.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.0/forwardkinematics/urdfFks/urdfFk.py` & `forwardkinematics-1.2.1/forwardkinematics/urdfFks/urdfFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.0/pyproject.toml` & `forwardkinematics-1.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "forwardkinematics"
-version = "1.2.0"
+version = "1.2.1"
 description = "\"Light-weight implementation of forward kinematics using casadi.\""
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maxspahn/forwardKinematics.git"
 repository = "https://github.com/maxspahn/forwardKinematics.git"
 
 
 [tool.poetry.dependencies]
 python = "^3.8,<4.0"
 casadi = "^3.5.4,!=3.5.5.post1,!=3.5.5.post2"
 numpy = "^1.15.3"
 urdf_parser_py = ">=0.0.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
 jedi = "^0.18.1"
 pytest = "^6.2.5"
 pytest-coverage = "^0.0"
 black = "^22.3.0"
 pylint = "^2.13.8"
 
 [build-system]
```

### Comparing `forwardkinematics-1.2.0/PKG-INFO` & `forwardkinematics-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forwardkinematics
-Version: 1.2.0
+Version: 1.2.1
 Summary: "Light-weight implementation of forward kinematics using casadi."
 Home-page: https://github.com/maxspahn/forwardKinematics.git
 License: MIT
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

