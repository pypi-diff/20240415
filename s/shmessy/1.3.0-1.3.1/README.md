# Comparing `tmp/shmessy-1.3.0.tar.gz` & `tmp/shmessy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shmessy-1.3.0.tar", max compression
+gzip compressed data, was "shmessy-1.3.1.tar", max compression
```

## Comparing `shmessy-1.3.0.tar` & `shmessy-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1073 2024-04-08 17:24:49.873855 shmessy-1.3.0/LICENSE
--rw-r--r--   0        0        0     5669 2024-04-08 17:24:49.873855 shmessy-1.3.0/README.md
--rw-r--r--   0        0        0      856 2024-04-08 17:25:19.726321 shmessy-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5701 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/__init__.py
--rw-r--r--   0        0        0     2023 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/exceptions.py
--rw-r--r--   0        0        0      395 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/schema.py
--rw-r--r--   0        0        0        0 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/base.py
--rw-r--r--   0        0        0     2226 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/boolean.py
--rw-r--r--   0        0        0     2493 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/date.py
--rw-r--r--   0        0        0     2929 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/datetime_.py
--rw-r--r--   0        0        0     1016 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/email.py
--rw-r--r--   0        0        0     1550 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/float.py
--rw-r--r--   0        0        0     1256 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/integer.py
--rw-r--r--   0        0        0     1272 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/ipv4_address.py
--rw-r--r--   0        0        0      991 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/string.py
--rw-r--r--   0        0        0     3188 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types/unix_timestamp.py
--rw-r--r--   0        0        0     7381 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/types_handler.py
--rw-r--r--   0        0        0     1848 2024-04-08 17:24:49.877855 shmessy-1.3.0/src/shmessy/utils.py
--rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 shmessy-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-15 07:22:16.219028 shmessy-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5669 2024-04-15 07:22:16.219028 shmessy-1.3.1/README.md
+-rw-r--r--   0        0        0      856 2024-04-15 07:22:50.530708 shmessy-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5701 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/__init__.py
+-rw-r--r--   0        0        0     2023 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/exceptions.py
+-rw-r--r--   0        0        0      395 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/schema.py
+-rw-r--r--   0        0        0        0 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/base.py
+-rw-r--r--   0        0        0     2226 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/boolean.py
+-rw-r--r--   0        0        0     2493 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/date.py
+-rw-r--r--   0        0        0     2975 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/datetime_.py
+-rw-r--r--   0        0        0     1016 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/email.py
+-rw-r--r--   0        0        0     1550 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/float.py
+-rw-r--r--   0        0        0     1256 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/integer.py
+-rw-r--r--   0        0        0     1272 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/ipv4_address.py
+-rw-r--r--   0        0        0      991 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/string.py
+-rw-r--r--   0        0        0     3188 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types/unix_timestamp.py
+-rw-r--r--   0        0        0     7381 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/types_handler.py
+-rw-r--r--   0        0        0     1848 2024-04-15 07:22:16.223028 shmessy-1.3.1/src/shmessy/utils.py
+-rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 shmessy-1.3.1/PKG-INFO
```

### Comparing `shmessy-1.3.0/LICENSE` & `shmessy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/README.md` & `shmessy-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/pyproject.toml` & `shmessy-1.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shmessy"
-version = "v1.3.0"
+version = "v1.3.1"
 description = "If your data is messy - Use Shmessy!"
 readme = "README.md"
 authors = ["Ohad Mata <ohadmata@gmail.com>"]
 homepage = "https://github.com/ohadmata/shmessy"
 repository = "https://github.com/ohadmata/shmessy"
 packages = [
     { include = "shmessy", from = "src" },
```

### Comparing `shmessy-1.3.0/src/shmessy/__init__.py` & `shmessy-1.3.1/src/shmessy/__init__.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/exceptions.py` & `shmessy-1.3.1/src/shmessy/exceptions.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types/base.py` & `shmessy-1.3.1/src/shmessy/types/base.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types/boolean.py` & `shmessy-1.3.1/src/shmessy/types/boolean.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types/date.py` & `shmessy-1.3.1/src/shmessy/types/date.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types/datetime_.py` & `shmessy-1.3.1/src/shmessy/types/datetime_.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         "%Y-%m-%dT%H:%M:%SZ",  # 2022-12-30T00:00:00Z
         "%Y-%m-%dT%H:%M:%S.%f",  # 2022-12-30T00:00:00.000
         "%Y-%m-%d %H:%M:%S.%fZ",  # 2022-12-30 00:00:00.000Z
         "%Y-%m-%d %H:%M:%S.%f",  # 2022-12-30 00:00:00.000
         "%Y-%m-%dT%H:%M:%S.%fZ",  # 2022-12-30T00:00:00.000Z
         "%Y-%m-%dT%H:%M:%S",  # 2022-12-30T00:00:00
         "%d/%m/%Y %H:%M",  # 30/12/2022 00:00
+        "%Y-%m-%d %H:%M",  # 2020-09-24 11:57
         "%Y-%m-%d %H:%M:%S %Z",  # 2020-09-24 11:57:27 UTC
     ]
 
     def validate(self, data: ndarray) -> Optional[InferredField]:
         if data.dtype.type == np.dtype("datetime64"):
             return InferredField(inferred_type=self.name)
```

### Comparing `shmessy-1.3.0/src/shmessy/types/email.py` & `shmessy-1.3.1/src/shmessy/types/email.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types/float.py` & `shmessy-1.3.1/src/shmessy/types/float.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types/integer.py` & `shmessy-1.3.1/src/shmessy/types/integer.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types/ipv4_address.py` & `shmessy-1.3.1/src/shmessy/types/ipv4_address.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types/string.py` & `shmessy-1.3.1/src/shmessy/types/string.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types/unix_timestamp.py` & `shmessy-1.3.1/src/shmessy/types/unix_timestamp.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/types_handler.py` & `shmessy-1.3.1/src/shmessy/types_handler.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/src/shmessy/utils.py` & `shmessy-1.3.1/src/shmessy/utils.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.0/PKG-INFO` & `shmessy-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shmessy
-Version: 1.3.0
+Version: 1.3.1
 Summary: If your data is messy - Use Shmessy!
 Home-page: https://github.com/ohadmata/shmessy
 Author: Ohad Mata
 Author-email: ohadmata@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

