# Comparing `tmp/omop_cdm-0.1.0.tar.gz` & `tmp/omop_cdm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omop_cdm-0.1.0.tar", max compression
+gzip compressed data, was "omop_cdm-0.1.1.tar", max compression
```

## Comparing `omop_cdm-0.1.0.tar` & `omop_cdm-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11357 2024-04-15 13:42:54.616481 omop_cdm-0.1.0/LICENSE
--rw-r--r--   0        0        0     1255 2024-04-15 13:42:54.618294 omop_cdm-0.1.0/README.md
--rw-r--r--   0        0        0     1189 2024-04-15 13:42:54.626168 omop_cdm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       49 2024-04-15 13:42:54.628921 omop_cdm-0.1.0/src/omop_cdm/__init__.py
--rw-r--r--   0        0        0     1716 2024-04-15 13:42:54.630413 omop_cdm-0.1.0/src/omop_cdm/constants.py
--rw-r--r--   0        0        0     1793 2024-04-15 13:42:54.631513 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/__init__.py
--rw-r--r--   0        0        0    48388 2024-04-15 13:42:54.632796 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/clinical_data.py
--rw-r--r--   0        0        0     3517 2024-04-15 13:42:54.635172 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/derived_elements.py
--rw-r--r--   0        0        0     6848 2024-04-15 13:42:54.635728 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/health_economics.py
--rw-r--r--   0        0        0     4083 2024-04-15 13:42:54.636659 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/health_system_data.py
--rw-r--r--   0        0        0     2009 2024-04-15 13:42:54.637215 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/metadata.py
--rw-r--r--   0        0        0    12025 2024-04-15 13:42:54.637982 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/vocabularies.py
--rw-r--r--   0        0        0     1791 2024-04-15 13:42:54.638755 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/__init__.py
--rw-r--r--   0        0        0    51433 2024-04-15 13:42:54.639523 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/clinical_data.py
--rw-r--r--   0        0        0     6501 2024-04-15 13:42:54.640434 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/derived_elements.py
--rw-r--r--   0        0        0     6845 2024-04-15 13:42:54.641062 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/health_economics.py
--rw-r--r--   0        0        0     4799 2024-04-15 13:42:54.641763 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/health_system_data.py
--rw-r--r--   0        0        0     3005 2024-04-15 13:42:54.643607 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/metadata.py
--rw-r--r--   0        0        0      414 2024-04-15 13:42:54.644218 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/vocabularies/__init__.py
--rw-r--r--   0        0        0    12250 2024-04-15 13:42:54.644872 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/vocabularies/vocabularies.py
--rw-r--r--   0        0        0     1793 2024-04-15 13:42:54.645500 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/__init__.py
--rw-r--r--   0        0        0    52512 2024-04-15 13:42:54.646377 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/clinical_data.py
--rw-r--r--   0        0        0     3562 2024-04-15 13:42:54.646959 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/derived_elements.py
--rw-r--r--   0        0        0     7476 2024-04-15 13:42:54.647480 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/health_economics.py
--rw-r--r--   0        0        0     5747 2024-04-15 13:42:54.648006 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/health_system_data.py
--rw-r--r--   0        0        0     2007 2024-04-15 13:42:54.648566 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/metadata.py
--rw-r--r--   0        0        0    12797 2024-04-15 13:42:54.649893 omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/vocabularies.py
--rw-r--r--   0        0        0      177 2024-04-15 13:42:54.650448 omop_cdm-0.1.0/src/omop_cdm/dynamic/legacy/__init__.py
--rw-r--r--   0        0        0     4218 2024-04-15 13:42:54.651003 omop_cdm-0.1.0/src/omop_cdm/dynamic/legacy/legacy.py
--rw-r--r--   0        0        0      313 2024-04-15 13:42:54.652619 omop_cdm-0.1.0/src/omop_cdm/dynamic/ruff.toml
--rw-r--r--   0        0        0     1747 2024-04-15 13:42:54.653639 omop_cdm-0.1.0/src/omop_cdm/regular/cdm531/__init__.py
--rw-r--r--   0        0        0    54730 2024-04-15 13:42:54.654544 omop_cdm-0.1.0/src/omop_cdm/regular/cdm531/tables.py
--rw-r--r--   0        0        0     1790 2024-04-15 13:42:54.655731 omop_cdm-0.1.0/src/omop_cdm/regular/cdm54/__init__.py
--rw-r--r--   0        0        0    60350 2024-04-15 13:42:54.656735 omop_cdm-0.1.0/src/omop_cdm/regular/cdm54/tables.py
--rw-r--r--   0        0        0     1769 2024-04-15 13:42:54.657506 omop_cdm-0.1.0/src/omop_cdm/regular/cdm600/__init__.py
--rw-r--r--   0        0        0    60351 2024-04-15 13:42:54.658242 omop_cdm-0.1.0/src/omop_cdm/regular/cdm600/tables.py
--rw-r--r--   0        0        0      250 2024-04-15 13:42:54.659132 omop_cdm-0.1.0/src/omop_cdm/regular/ruff.toml
--rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 omop_cdm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-15 21:44:25.544504 omop_cdm-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1255 2024-04-15 21:44:25.544504 omop_cdm-0.1.1/README.md
+-rw-r--r--   0        0        0     1189 2024-04-15 21:44:25.544504 omop_cdm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-04-15 21:44:25.544504 omop_cdm-0.1.1/src/omop_cdm/__init__.py
+-rw-r--r--   0        0        0     1716 2024-04-15 21:44:25.544504 omop_cdm-0.1.1/src/omop_cdm/constants.py
+-rw-r--r--   0        0        0     1793 2024-04-15 21:44:25.544504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/__init__.py
+-rw-r--r--   0        0        0    48388 2024-04-15 21:44:25.544504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/clinical_data.py
+-rw-r--r--   0        0        0     3517 2024-04-15 21:44:25.544504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/derived_elements.py
+-rw-r--r--   0        0        0     6848 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/health_economics.py
+-rw-r--r--   0        0        0     4083 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/health_system_data.py
+-rw-r--r--   0        0        0     2009 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/metadata.py
+-rw-r--r--   0        0        0    12025 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/vocabularies.py
+-rw-r--r--   0        0        0     1791 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/__init__.py
+-rw-r--r--   0        0        0    51433 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/clinical_data.py
+-rw-r--r--   0        0        0     6501 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/derived_elements.py
+-rw-r--r--   0        0        0     6845 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/health_economics.py
+-rw-r--r--   0        0        0     4799 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/health_system_data.py
+-rw-r--r--   0        0        0     3005 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/metadata.py
+-rw-r--r--   0        0        0      414 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/vocabularies/__init__.py
+-rw-r--r--   0        0        0    12250 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/vocabularies/vocabularies.py
+-rw-r--r--   0        0        0     1793 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/__init__.py
+-rw-r--r--   0        0        0    52512 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/clinical_data.py
+-rw-r--r--   0        0        0     3562 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/derived_elements.py
+-rw-r--r--   0        0        0     7476 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/health_economics.py
+-rw-r--r--   0        0        0     5747 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/health_system_data.py
+-rw-r--r--   0        0        0     2007 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/metadata.py
+-rw-r--r--   0        0        0    12797 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/vocabularies.py
+-rw-r--r--   0        0        0      177 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/legacy/__init__.py
+-rw-r--r--   0        0        0     4218 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/legacy/legacy.py
+-rw-r--r--   0        0        0      313 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/dynamic/ruff.toml
+-rw-r--r--   0        0        0     1747 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/regular/cdm531/__init__.py
+-rw-r--r--   0        0        0    54730 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/regular/cdm531/tables.py
+-rw-r--r--   0        0        0     1790 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/regular/cdm54/__init__.py
+-rw-r--r--   0        0        0    60350 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/regular/cdm54/tables.py
+-rw-r--r--   0        0        0     1769 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/regular/cdm600/__init__.py
+-rw-r--r--   0        0        0    60351 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/regular/cdm600/tables.py
+-rw-r--r--   0        0        0      250 2024-04-15 21:44:25.548504 omop_cdm-0.1.1/src/omop_cdm/regular/ruff.toml
+-rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 omop_cdm-0.1.1/PKG-INFO
```

### Comparing `omop_cdm-0.1.0/LICENSE` & `omop_cdm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/README.md` & `omop_cdm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/pyproject.toml` & `omop_cdm-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omop-cdm"
-version = "0.1.0"
+version = "0.1.1"
 description = "SQLAlchemy ORM of the OHDSI OMOP CDM"
 authors = [
     "Spayralbe <stefan@thehyve.nl>",
 ]
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `omop_cdm-0.1.0/src/omop_cdm/constants.py` & `omop_cdm-0.1.1/src/omop_cdm/constants.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/__init__.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/__init__.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/clinical_data.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/clinical_data.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/derived_elements.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/derived_elements.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/health_economics.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/health_economics.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/health_system_data.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/health_system_data.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/metadata.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/metadata.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm531/vocabularies.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm531/vocabularies.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/__init__.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/__init__.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/clinical_data.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/clinical_data.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/derived_elements.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/derived_elements.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/health_economics.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/health_economics.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/health_system_data.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/health_system_data.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/metadata.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/metadata.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm54/vocabularies/vocabularies.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm54/vocabularies/vocabularies.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/__init__.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/__init__.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/clinical_data.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/clinical_data.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/derived_elements.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/derived_elements.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/health_economics.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/health_economics.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/health_system_data.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/health_system_data.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/metadata.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/metadata.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/cdm600/vocabularies.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/cdm600/vocabularies.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/dynamic/legacy/legacy.py` & `omop_cdm-0.1.1/src/omop_cdm/dynamic/legacy/legacy.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/regular/cdm531/__init__.py` & `omop_cdm-0.1.1/src/omop_cdm/regular/cdm531/__init__.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/regular/cdm531/tables.py` & `omop_cdm-0.1.1/src/omop_cdm/regular/cdm531/tables.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/regular/cdm54/__init__.py` & `omop_cdm-0.1.1/src/omop_cdm/regular/cdm54/__init__.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/regular/cdm54/tables.py` & `omop_cdm-0.1.1/src/omop_cdm/regular/cdm54/tables.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/regular/cdm600/__init__.py` & `omop_cdm-0.1.1/src/omop_cdm/regular/cdm600/__init__.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/src/omop_cdm/regular/cdm600/tables.py` & `omop_cdm-0.1.1/src/omop_cdm/regular/cdm600/tables.py`

 * *Files identical despite different names*

### Comparing `omop_cdm-0.1.0/PKG-INFO` & `omop_cdm-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omop-cdm
-Version: 0.1.0
+Version: 0.1.1
 Summary: SQLAlchemy ORM of the OHDSI OMOP CDM
 Author: Spayralbe
 Author-email: stefan@thehyve.nl
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

