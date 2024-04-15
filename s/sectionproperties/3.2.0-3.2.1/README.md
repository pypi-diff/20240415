# Comparing `tmp/sectionproperties-3.2.0.tar.gz` & `tmp/sectionproperties-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sectionproperties-3.2.0.tar", max compression
+gzip compressed data, was "sectionproperties-3.2.1.tar", max compression
```

## Comparing `sectionproperties-3.2.0.tar` & `sectionproperties-3.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1074 2024-03-09 20:48:26.175691 sectionproperties-3.2.0/LICENSE
--rw-r--r--   0        0        0     4155 2024-03-09 20:48:26.175691 sectionproperties-3.2.0/README.md
--rw-r--r--   0        0        0     4386 2024-03-09 20:48:37.643655 sectionproperties-3.2.0/pyproject.toml
--rw-r--r--   0        0        0      353 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/__init__.py
--rw-r--r--   0        0        0      225 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/__main__.py
--rw-r--r--   0        0        0       97 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/analysis/__init__.py
--rw-r--r--   0        0        0    40040 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/analysis/fea.py
--rw-r--r--   0        0        0    15869 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/analysis/plastic_section.py
--rw-r--r--   0        0        0   126376 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/analysis/section.py
--rw-r--r--   0        0        0     5423 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/analysis/solver.py
--rw-r--r--   0        0        0       40 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/post/__init__.py
--rw-r--r--   0        0        0     6406 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/post/fibre.py
--rw-r--r--   0        0        0    31352 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/post/post.py
--rw-r--r--   0        0        0    40740 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/post/stress_post.py
--rw-r--r--   0        0        0      157 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/__init__.py
--rw-r--r--   0        0        0     3718 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/bisect_section.py
--rw-r--r--   0        0        0   106318 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/geometry.py
--rw-r--r--   0        0        0     1486 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/library/__init__.py
--rw-r--r--   0        0        0     8677 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/library/bridge_sections.py
--rw-r--r--   0        0        0    23678 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/library/concrete_sections.py
--rw-r--r--   0        0        0    46245 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/library/nastran_sections.py
--rw-r--r--   0        0        0     9883 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/library/primitive_sections.py
--rw-r--r--   0        0        0    49709 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/library/steel_sections.py
--rw-r--r--   0        0        0     1781 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/library/utils.py
--rw-r--r--   0        0        0     5020 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/pre.py
--rw-r--r--   0        0        0     5041 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/pre/rhino.py
--rw-r--r--   0        0        0        0 2024-03-09 20:48:26.199691 sectionproperties-3.2.0/src/sectionproperties/py.typed
--rw-r--r--   0        0        0    22125 2024-03-09 20:48:26.203691 sectionproperties-3.2.0/tests/geometry/complex_shape.txt
--rw-r--r--   0        0        0    24105 2024-03-09 20:48:26.203691 sectionproperties-3.2.0/tests/geometry/compound_shape.txt
--rw-r--r--   0        0        0     6505 1970-01-01 00:00:00.000000 sectionproperties-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-15 00:54:11.020640 sectionproperties-3.2.1/LICENSE
+-rw-r--r--   0        0        0     4155 2024-04-15 00:54:11.020640 sectionproperties-3.2.1/README.md
+-rw-r--r--   0        0        0     4386 2024-04-15 00:54:21.876767 sectionproperties-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0      353 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/__main__.py
+-rw-r--r--   0        0        0       97 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/__init__.py
+-rw-r--r--   0        0        0    40040 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/fea.py
+-rw-r--r--   0        0        0    15869 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/plastic_section.py
+-rw-r--r--   0        0        0   126376 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/section.py
+-rw-r--r--   0        0        0     5423 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/solver.py
+-rw-r--r--   0        0        0       40 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/post/__init__.py
+-rw-r--r--   0        0        0     6406 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/post/fibre.py
+-rw-r--r--   0        0        0    31352 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/post/post.py
+-rw-r--r--   0        0        0    40740 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/post/stress_post.py
+-rw-r--r--   0        0        0      157 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/__init__.py
+-rw-r--r--   0        0        0     3718 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/bisect_section.py
+-rw-r--r--   0        0        0   106318 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/geometry.py
+-rw-r--r--   0        0        0     1486 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/__init__.py
+-rw-r--r--   0        0        0     8677 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/bridge_sections.py
+-rw-r--r--   0        0        0    23678 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/concrete_sections.py
+-rw-r--r--   0        0        0    46245 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/nastran_sections.py
+-rw-r--r--   0        0        0     9883 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/primitive_sections.py
+-rw-r--r--   0        0        0    49709 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/steel_sections.py
+-rw-r--r--   0        0        0     1781 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/utils.py
+-rw-r--r--   0        0        0     5020 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/pre.py
+-rw-r--r--   0        0        0     5041 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/rhino.py
+-rw-r--r--   0        0        0        0 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/py.typed
+-rw-r--r--   0        0        0    22125 2024-04-15 00:54:11.044640 sectionproperties-3.2.1/tests/geometry/complex_shape.txt
+-rw-r--r--   0        0        0    24105 2024-04-15 00:54:11.044640 sectionproperties-3.2.1/tests/geometry/compound_shape.txt
+-rw-r--r--   0        0        0     6505 1970-01-01 00:00:00.000000 sectionproperties-3.2.1/PKG-INFO
```

### Comparing `sectionproperties-3.2.0/LICENSE` & `sectionproperties-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/README.md` & `sectionproperties-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/pyproject.toml` & `sectionproperties-3.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sectionproperties"
-version = "3.2.0"
+version = "3.2.1"
 description = "A python package for the analysis of arbitrary cross-sections using the finite element method."
 license = "MIT"
 authors = [
     "Robbie van Leeuwen <robbie.vanleeuwen@gmail.com>",
 ]
 maintainers = [
     "Robbie van Leeuwen <robbie.vanleeuwen@gmail.com>",
```

### Comparing `sectionproperties-3.2.0/src/sectionproperties/analysis/fea.py` & `sectionproperties-3.2.1/src/sectionproperties/analysis/fea.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/analysis/plastic_section.py` & `sectionproperties-3.2.1/src/sectionproperties/analysis/plastic_section.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/analysis/section.py` & `sectionproperties-3.2.1/src/sectionproperties/analysis/section.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/analysis/solver.py` & `sectionproperties-3.2.1/src/sectionproperties/analysis/solver.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/post/fibre.py` & `sectionproperties-3.2.1/src/sectionproperties/post/fibre.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/post/post.py` & `sectionproperties-3.2.1/src/sectionproperties/post/post.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/post/stress_post.py` & `sectionproperties-3.2.1/src/sectionproperties/post/stress_post.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/bisect_section.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/bisect_section.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/geometry.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/geometry.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/library/__init__.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/library/__init__.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/library/bridge_sections.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/library/bridge_sections.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/library/concrete_sections.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/library/concrete_sections.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/library/nastran_sections.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/library/nastran_sections.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/library/primitive_sections.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/library/primitive_sections.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/library/steel_sections.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/library/steel_sections.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/library/utils.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/library/utils.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/pre.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/pre.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/src/sectionproperties/pre/rhino.py` & `sectionproperties-3.2.1/src/sectionproperties/pre/rhino.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/tests/geometry/complex_shape.txt` & `sectionproperties-3.2.1/tests/geometry/complex_shape.txt`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/tests/geometry/compound_shape.txt` & `sectionproperties-3.2.1/tests/geometry/compound_shape.txt`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.0/PKG-INFO` & `sectionproperties-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectionproperties
-Version: 3.2.0
+Version: 3.2.1
 Summary: A python package for the analysis of arbitrary cross-sections using the finite element method.
 Home-page: https://github.com/robbievanleeuwen/section-properties
 License: MIT
 Keywords: cross-section,structural-engineering,finite-element-analysis,computational-mechanics
 Author: Robbie van Leeuwen
 Author-email: robbie.vanleeuwen@gmail.com
 Maintainer: Robbie van Leeuwen
```

