# Comparing `tmp/serialzy-1.5.1.tar.gz` & `tmp/serialzy-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialzy-1.5.1.tar", last modified: Thu Feb 22 17:11:19 2024, max compression
+gzip compressed data, was "serialzy-1.5.2.tar", last modified: Mon Apr 15 18:42:39 2024, max compression
```

## Comparing `serialzy-1.5.1.tar` & `serialzy-1.5.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 aapurii  (1039082238) LD\Domain Users (593637566)        0 2024-02-22 17:11:19.500830 serialzy-1.5.1/
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)      659 2024-02-16 07:27:53.000000 serialzy-1.5.1/AUTHORS
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)      578 2024-02-16 07:27:53.000000 serialzy-1.5.1/LICENSE
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)       40 2024-02-16 07:27:53.000000 serialzy-1.5.1/MANIFEST.in
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     7938 2024-02-22 17:11:19.500727 serialzy-1.5.1/PKG-INFO
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     7485 2024-02-16 07:27:53.000000 serialzy-1.5.1/README.md
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)      345 2024-02-21 14:21:46.000000 serialzy-1.5.1/pyproject.toml
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)       43 2024-02-16 07:27:53.000000 serialzy-1.5.1/requirements.txt
-drwxr-xr-x   0 aapurii  (1039082238) LD\Domain Users (593637566)        0 2024-02-22 17:11:19.497602 serialzy-1.5.1/serialzy/
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)       60 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/__init__.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     8468 2024-02-21 18:56:56.000000 serialzy-1.5.1/serialzy/api.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     3014 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/base.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     2180 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/cloudpickle.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)       41 2024-02-16 07:27:53.000000 serialzy-1.5.1/serialzy/errors.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     2149 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/exception.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     8255 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/registry.py
-drwxr-xr-x   0 aapurii  (1039082238) LD\Domain Users (593637566)        0 2024-02-22 17:11:19.500394 serialzy-1.5.1/serialzy/serializers/
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)        0 2024-02-16 07:27:53.000000 serialzy-1.5.1/serialzy/serializers/__init__.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     7234 2024-02-22 16:14:13.000000 serialzy-1.5.1/serialzy/serializers/base_model.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     2588 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/catboost.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     1562 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/ellipsis.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     1273 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/lightgbm.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     1643 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/onnx.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     1385 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/primitive.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     2830 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/proto.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     7446 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/sequence.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     1937 2024-02-22 16:42:40.000000 serialzy-1.5.1/serialzy/serializers/sklearn.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     3355 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/tensorflow.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     1288 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/torch.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     6499 2024-02-21 18:56:56.000000 serialzy-1.5.1/serialzy/serializers/union.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     1368 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/serializers/xgboost.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     1317 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/types.py
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)      851 2024-02-21 14:21:42.000000 serialzy-1.5.1/serialzy/utils.py
-drwxr-xr-x   0 aapurii  (1039082238) LD\Domain Users (593637566)        0 2024-02-22 17:11:19.500548 serialzy-1.5.1/serialzy/version/
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)        6 2024-02-22 14:19:43.000000 serialzy-1.5.1/serialzy/version/version
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)      129 2024-02-16 07:27:53.000000 serialzy-1.5.1/serialzy/version.py
-drwxr-xr-x   0 aapurii  (1039082238) LD\Domain Users (593637566)        0 2024-02-22 17:11:19.498149 serialzy-1.5.1/serialzy.egg-info/
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     7938 2024-02-22 17:11:19.000000 serialzy-1.5.1/serialzy.egg-info/PKG-INFO
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)      910 2024-02-22 17:11:19.000000 serialzy-1.5.1/serialzy.egg-info/SOURCES.txt
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)        1 2024-02-22 17:11:19.000000 serialzy-1.5.1/serialzy.egg-info/dependency_links.txt
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)       43 2024-02-22 17:11:19.000000 serialzy-1.5.1/serialzy.egg-info/requires.txt
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)       30 2024-02-22 17:11:19.000000 serialzy-1.5.1/serialzy.egg-info/top_level.txt
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)       38 2024-02-22 17:11:19.500872 serialzy-1.5.1/setup.cfg
--rw-r--r--   0 aapurii  (1039082238) LD\Domain Users (593637566)     1156 2024-02-16 07:27:53.000000 serialzy-1.5.1/setup.py
+drwxrwxr-x   0 imakunin  (1000) imakunin  (1000)        0 2024-04-15 18:42:39.714907 serialzy-1.5.2/
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)      659 2023-06-30 14:01:32.000000 serialzy-1.5.2/AUTHORS
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)      578 2023-06-30 14:01:32.000000 serialzy-1.5.2/LICENSE
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)       40 2023-06-30 14:01:32.000000 serialzy-1.5.2/MANIFEST.in
+-rw-r--r--   0 imakunin  (1000) imakunin  (1000)     8011 2024-04-15 18:42:39.714907 serialzy-1.5.2/PKG-INFO
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     7485 2023-11-03 13:31:41.000000 serialzy-1.5.2/README.md
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)      345 2023-09-27 07:39:36.000000 serialzy-1.5.2/pyproject.toml
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)       43 2023-08-24 11:05:20.000000 serialzy-1.5.2/requirements.txt
+drwxrwxr-x   0 imakunin  (1000) imakunin  (1000)        0 2024-04-15 18:42:39.710907 serialzy-1.5.2/serialzy/
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)       60 2023-09-27 07:39:36.000000 serialzy-1.5.2/serialzy/__init__.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     8468 2024-02-22 08:24:12.000000 serialzy-1.5.2/serialzy/api.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     3014 2023-10-06 10:13:20.000000 serialzy-1.5.2/serialzy/base.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     2180 2023-09-27 07:39:36.000000 serialzy-1.5.2/serialzy/cloudpickle.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)       41 2023-06-30 14:01:32.000000 serialzy-1.5.2/serialzy/errors.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     2149 2023-09-27 07:39:36.000000 serialzy-1.5.2/serialzy/exception.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     8255 2023-10-05 10:11:30.000000 serialzy-1.5.2/serialzy/registry.py
+drwxrwxr-x   0 imakunin  (1000) imakunin  (1000)        0 2024-04-15 18:42:39.714907 serialzy-1.5.2/serialzy/serializers/
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)        0 2023-06-30 14:01:32.000000 serialzy-1.5.2/serialzy/serializers/__init__.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     7205 2024-04-15 18:41:22.000000 serialzy-1.5.2/serialzy/serializers/base_model.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     2588 2023-10-05 08:52:24.000000 serialzy-1.5.2/serialzy/serializers/catboost.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     1562 2023-06-30 14:01:32.000000 serialzy-1.5.2/serialzy/serializers/ellipsis.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     1273 2023-09-27 07:39:36.000000 serialzy-1.5.2/serialzy/serializers/lightgbm.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     1643 2023-11-03 13:31:41.000000 serialzy-1.5.2/serialzy/serializers/onnx.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     1385 2023-09-27 07:39:36.000000 serialzy-1.5.2/serialzy/serializers/primitive.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     2830 2023-09-27 07:39:36.000000 serialzy-1.5.2/serialzy/serializers/proto.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     7446 2023-06-30 14:01:32.000000 serialzy-1.5.2/serialzy/serializers/sequence.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     1937 2024-04-15 12:48:04.000000 serialzy-1.5.2/serialzy/serializers/sklearn.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     3867 2024-04-15 18:41:22.000000 serialzy-1.5.2/serialzy/serializers/tensorflow.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     1288 2023-09-27 07:39:36.000000 serialzy-1.5.2/serialzy/serializers/torch.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     6499 2024-02-22 08:24:12.000000 serialzy-1.5.2/serialzy/serializers/union.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     1368 2023-09-27 07:39:36.000000 serialzy-1.5.2/serialzy/serializers/xgboost.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     1317 2023-06-30 14:01:32.000000 serialzy-1.5.2/serialzy/types.py
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)      851 2023-09-27 07:39:36.000000 serialzy-1.5.2/serialzy/utils.py
+drwxrwxr-x   0 imakunin  (1000) imakunin  (1000)        0 2024-04-15 18:42:39.714907 serialzy-1.5.2/serialzy/version/
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)        6 2024-04-15 18:41:22.000000 serialzy-1.5.2/serialzy/version/version
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)      129 2023-06-30 14:01:32.000000 serialzy-1.5.2/serialzy/version.py
+drwxrwxr-x   0 imakunin  (1000) imakunin  (1000)        0 2024-04-15 18:42:39.714907 serialzy-1.5.2/serialzy.egg-info/
+-rw-r--r--   0 imakunin  (1000) imakunin  (1000)     8011 2024-04-15 18:42:39.000000 serialzy-1.5.2/serialzy.egg-info/PKG-INFO
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)      910 2024-04-15 18:42:39.000000 serialzy-1.5.2/serialzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)        1 2024-04-15 18:42:39.000000 serialzy-1.5.2/serialzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)       43 2024-04-15 18:42:39.000000 serialzy-1.5.2/serialzy.egg-info/requires.txt
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)       30 2024-04-15 18:42:39.000000 serialzy-1.5.2/serialzy.egg-info/top_level.txt
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)       38 2024-04-15 18:42:39.714907 serialzy-1.5.2/setup.cfg
+-rw-rw-r--   0 imakunin  (1000) imakunin  (1000)     1156 2023-09-27 07:46:09.000000 serialzy-1.5.2/setup.py
```

### Comparing `serialzy-1.5.1/AUTHORS` & `serialzy-1.5.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/LICENSE` & `serialzy-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/PKG-INFO` & `serialzy-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: serialzy
-Version: 1.5.1
+Version: 1.5.2
 Author: ʎzy developers
 License: LICENSE
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: packaging>=21.3.0
+Requires-Dist: typing-extensions>=4.4.0
 
 [![Pypi version](https://img.shields.io/pypi/v/serialzy)](https://pypi.org/project/serialzy/)
 [![Tests](https://github.com/lambdazy/serialzy/actions/workflows/tests.yaml/badge.svg)](https://github.com/lambda-zy/lzy/actions/workflows/tests.yaml)
 [![Python tests coverage](https://gist.githubusercontent.com/mrMakaronka/74a3e00f914bb55c0f3582a7d48e3bcd/raw/main-coverage.svg)](https://github.com/lambdazy/lzy/tree/master/pylzy/tests)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/serialzy.svg)](https://pypi.org/project/serialzy/)
 
 # serialzy
```

### Comparing `serialzy-1.5.1/README.md` & `serialzy-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/api.py` & `serialzy-1.5.2/serialzy/api.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/base.py` & `serialzy-1.5.2/serialzy/base.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/cloudpickle.py` & `serialzy-1.5.2/serialzy/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/exception.py` & `serialzy-1.5.2/serialzy/exception.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/registry.py` & `serialzy-1.5.2/serialzy/registry.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/base_model.py` & `serialzy-1.5.2/serialzy/serializers/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,15 @@
     def __check_module_fits_serializer(self, typ: Type) -> bool:
         name = module_name(typ)
         if name == self.module:
             return True
 
         if hasattr(typ, '__bases__'):
             for base in typ.__bases__:
-                base_name = module_name(base)
-                if base_name == self.module:
+                if self.__check_module_fits_serializer(base):
                     return True
         return False
 
     def serialize_with_meta(self, obj: Any, dest_dir: str, model_file_name: str) -> None:
         """
         :param obj: object to serialize into bytes
         :param dest_dir: files with serialized model and meta are written into destination directory
```

### Comparing `serialzy-1.5.1/serialzy/serializers/catboost.py` & `serialzy-1.5.2/serialzy/serializers/catboost.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/ellipsis.py` & `serialzy-1.5.2/serialzy/serializers/ellipsis.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/lightgbm.py` & `serialzy-1.5.2/serialzy/serializers/lightgbm.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/onnx.py` & `serialzy-1.5.2/serialzy/serializers/onnx.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/primitive.py` & `serialzy-1.5.2/serialzy/serializers/primitive.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/proto.py` & `serialzy-1.5.2/serialzy/serializers/proto.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/sequence.py` & `serialzy-1.5.2/serialzy/serializers/sequence.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/sklearn.py` & `serialzy-1.5.2/serialzy/serializers/sklearn.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/tensorflow.py` & `serialzy-1.5.2/serialzy/serializers/tensorflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,30 @@
 
 
 # noinspection PyPackageRequirements
 class TensorflowKerasSerializer(ModelBaseSerializer):
     def __init__(self):
         super().__init__("keras", __name__)
 
+    def available(self) -> bool:
+        available = super().available()
+        if not available:
+            return False
+
+        import keras
+        version = getattr(keras, '__version__', None)  # keras < 1 doesn't have this field
+
+        # I don't like this string comparison, version 13.0.0 says hi
+        # TODO: remake to packaging.version
+        if version and (version < '3.0.0'):
+            return True
+
+        self.logger.warning('Unsupported keras version %s', version)
+        return False
+
     def unpack_model(self, source: BinaryIO, dest_dir: Union[str, PathLike]) -> PathLike:
         model_path = Path(dest_dir) / "model.savedmodel"
         unpack_model_tar(source, model_path)
         return model_path
 
     def data_format(self) -> str:
         return "tf_keras"
```

### Comparing `serialzy-1.5.1/serialzy/serializers/torch.py` & `serialzy-1.5.2/serialzy/serializers/torch.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/union.py` & `serialzy-1.5.2/serialzy/serializers/union.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/serializers/xgboost.py` & `serialzy-1.5.2/serialzy/serializers/xgboost.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/types.py` & `serialzy-1.5.2/serialzy/types.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy/utils.py` & `serialzy-1.5.2/serialzy/utils.py`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/serialzy.egg-info/PKG-INFO` & `serialzy-1.5.2/serialzy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: serialzy
-Version: 1.5.1
+Version: 1.5.2
 Author: ʎzy developers
 License: LICENSE
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: packaging>=21.3.0
+Requires-Dist: typing-extensions>=4.4.0
 
 [![Pypi version](https://img.shields.io/pypi/v/serialzy)](https://pypi.org/project/serialzy/)
 [![Tests](https://github.com/lambdazy/serialzy/actions/workflows/tests.yaml/badge.svg)](https://github.com/lambda-zy/lzy/actions/workflows/tests.yaml)
 [![Python tests coverage](https://gist.githubusercontent.com/mrMakaronka/74a3e00f914bb55c0f3582a7d48e3bcd/raw/main-coverage.svg)](https://github.com/lambdazy/lzy/tree/master/pylzy/tests)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/serialzy.svg)](https://pypi.org/project/serialzy/)
 
 # serialzy
```

### Comparing `serialzy-1.5.1/serialzy.egg-info/SOURCES.txt` & `serialzy-1.5.2/serialzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serialzy-1.5.1/setup.py` & `serialzy-1.5.2/setup.py`

 * *Files identical despite different names*

