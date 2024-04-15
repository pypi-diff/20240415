# Comparing `tmp/kyoslib_py-5.1.0.tar.gz` & `tmp/kyoslib_py-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyoslib_py-5.1.0.tar", max compression
+gzip compressed data, was "kyoslib_py-5.1.1.tar", max compression
```

## Comparing `kyoslib_py-5.1.0.tar` & `kyoslib_py-5.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2024-03-28 13:16:58.303035 kyoslib_py-5.1.0/LICENSE.txt
--rw-r--r--   0        0        0      945 2024-03-28 13:16:58.303035 kyoslib_py-5.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/__init__.py
--rw-r--r--   0        0        0    10927 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/forward_curve.py
--rw-r--r--   0        0        0    15661 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/front_end.py
--rw-r--r--   0        0        0    24439 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/historical_price.py
--rw-r--r--   0        0        0     3459 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/kyos_api.py
--rw-r--r--   0        0        0     4554 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/kyos_utils.py
--rw-r--r--   0        0        0    45398 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/settings.py
--rw-r--r--   0        0        0    94919 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/simulation.py
--rw-r--r--   0        0        0    21239 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/tradable_product.py
--rw-r--r--   0        0        0    36070 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/kyoslib_py/valuation_interface.py
--rw-r--r--   0        0        0     1116 2024-03-28 13:16:58.311035 kyoslib_py-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 kyoslib_py-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-15 08:11:17.960159 kyoslib_py-5.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      945 2024-04-15 08:11:17.960159 kyoslib_py-5.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/__init__.py
+-rw-r--r--   0        0        0    10927 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/forward_curve.py
+-rw-r--r--   0        0        0    15661 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/front_end.py
+-rw-r--r--   0        0        0    24439 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/historical_price.py
+-rw-r--r--   0        0        0     3459 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/kyos_api.py
+-rw-r--r--   0        0        0     4554 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/kyos_utils.py
+-rw-r--r--   0        0        0    45398 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/settings.py
+-rw-r--r--   0        0        0    94919 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/simulation.py
+-rw-r--r--   0        0        0    21239 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/tradable_product.py
+-rw-r--r--   0        0        0    36070 2024-04-15 08:11:17.968159 kyoslib_py-5.1.1/kyoslib_py/valuation_interface.py
+-rw-r--r--   0        0        0     1116 2024-04-15 08:11:17.968159 kyoslib_py-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 kyoslib_py-5.1.1/PKG-INFO
```

### Comparing `kyoslib_py-5.1.0/LICENSE.txt` & `kyoslib_py-5.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/README.md` & `kyoslib_py-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/kyoslib_py/forward_curve.py` & `kyoslib_py-5.1.1/kyoslib_py/forward_curve.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/kyoslib_py/front_end.py` & `kyoslib_py-5.1.1/kyoslib_py/front_end.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/kyoslib_py/historical_price.py` & `kyoslib_py-5.1.1/kyoslib_py/historical_price.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/kyoslib_py/kyos_api.py` & `kyoslib_py-5.1.1/kyoslib_py/kyos_api.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/kyoslib_py/kyos_utils.py` & `kyoslib_py-5.1.1/kyoslib_py/kyos_utils.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/kyoslib_py/settings.py` & `kyoslib_py-5.1.1/kyoslib_py/settings.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/kyoslib_py/simulation.py` & `kyoslib_py-5.1.1/kyoslib_py/simulation.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/kyoslib_py/tradable_product.py` & `kyoslib_py-5.1.1/kyoslib_py/tradable_product.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/kyoslib_py/valuation_interface.py` & `kyoslib_py-5.1.1/kyoslib_py/valuation_interface.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.0/pyproject.toml` & `kyoslib_py-5.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kyoslib_py"
-version = "5.1.0"
+version = "5.1.1"
 description = "KYOS shared lib code as python package"
 authors = ["KYOS <support@kyos.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/kyosenergy/kyoslib_py"
 documentation = "https://kyosenergy.github.io/kyoslib_py/"
```

### Comparing `kyoslib_py-5.1.0/PKG-INFO` & `kyoslib_py-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kyoslib_py
-Version: 5.1.0
+Version: 5.1.1
 Summary: KYOS shared lib code as python package
 Home-page: http://github.com/kyosenergy/kyoslib_py
 License: MIT
 Author: KYOS
 Author-email: support@kyos.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

