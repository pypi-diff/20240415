# Comparing `tmp/dapla_toolbelt_pseudo-1.8.4.tar.gz` & `tmp/dapla_toolbelt_pseudo-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-1.8.4.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-1.8.5.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-1.8.4.tar` & `dapla_toolbelt_pseudo-1.8.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2024-04-11 21:39:16.938192 dapla_toolbelt_pseudo-1.8.4/LICENSE
--rw-r--r--   0        0        0    17053 2024-04-11 21:39:16.938192 dapla_toolbelt_pseudo-1.8.4/README.md
--rw-r--r--   0        0        0     4728 2024-04-11 21:39:26.422189 dapla_toolbelt_pseudo-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     1493 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1763 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      994 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/exceptions.py
--rw-r--r--   0        0        0      847 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      828 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0     2115 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      543 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0    12531 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/api_models.py
--rw-r--r--   0        0        0     2974 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/baseclass.py
--rw-r--r--   0        0        0     6118 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0    15341 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/depseudo.py
--rw-r--r--   0        0        0    15621 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/pseudo.py
--rw-r--r--   0        0        0     9346 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/pseudo_commons.py
--rw-r--r--   0        0        0    19278 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/repseudo.py
--rw-r--r--   0        0        0     8330 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/result.py
--rw-r--r--   0        0        0     4188 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     5611 2024-04-11 21:39:16.942192 dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/validation.py
--rw-r--r--   0        0        0    18503 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-15 06:30:14.054759 dapla_toolbelt_pseudo-1.8.5/LICENSE
+-rw-r--r--   0        0        0    17053 2024-04-15 06:30:14.054759 dapla_toolbelt_pseudo-1.8.5/README.md
+-rw-r--r--   0        0        0     4728 2024-04-15 06:30:27.778695 dapla_toolbelt_pseudo-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0     1493 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1763 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      994 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/exceptions.py
+-rw-r--r--   0        0        0      847 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      828 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0     2115 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      543 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0    12531 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/api_models.py
+-rw-r--r--   0        0        0     2974 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/baseclass.py
+-rw-r--r--   0        0        0     6118 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0    15341 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/depseudo.py
+-rw-r--r--   0        0        0    15621 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/pseudo.py
+-rw-r--r--   0        0        0     9346 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/pseudo_commons.py
+-rw-r--r--   0        0        0    19278 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/repseudo.py
+-rw-r--r--   0        0        0     8347 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/result.py
+-rw-r--r--   0        0        0     4188 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     5611 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/validation.py
+-rw-r--r--   0        0        0    18503 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.8.5/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-1.8.4/LICENSE` & `dapla_toolbelt_pseudo-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/README.md` & `dapla_toolbelt_pseudo-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/pyproject.toml` & `dapla_toolbelt_pseudo-1.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "1.8.4"
+version = "1.8.5"
 description = "Pseudonymization extensions for Dapla"
 authors = ["Dapla Developers <dapla-platform-developers@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
```

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/constants.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/exceptions.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/types.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/types.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/__init__.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/api_models.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/api_models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/baseclass.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/baseclass.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/client.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/depseudo.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/depseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/pseudo.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/pseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/pseudo_commons.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/pseudo_commons.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/repseudo.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/repseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/result.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     @property
     def datadoc(self) -> str:
         """Returns the pseudonymization metadata as a dictionary.
 
         Returns:
             str: A JSON-formattted string representing the datadoc metadata.
         """
-        return self._datadoc.model_dump_json()
+        return self._datadoc.model_dump_json(exclude_none=True)
 
     def _datadoc_from_raw_metadata_fields(
         self,
         raw_metadata: list[dict[str, Any]],
     ) -> PseudoVariable | None:
         if len(raw_metadata) == 0:
             return None
```

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/src/dapla_pseudo/v1/validation.py` & `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/validation.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.4/PKG-INFO` & `dapla_toolbelt_pseudo-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 1.8.4
+Version: 1.8.5
 Summary: Pseudonymization extensions for Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Dapla Developers
 Author-email: dapla-platform-developers@ssb.no
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
```

