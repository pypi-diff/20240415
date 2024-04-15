# Comparing `tmp/types_awscrt-0.20.5.tar.gz` & `tmp/types_awscrt-0.20.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types_awscrt-0.20.5.tar", max compression
+gzip compressed data, was "types_awscrt-0.20.7.tar", max compression
```

## Comparing `types_awscrt-0.20.5.tar` & `types_awscrt-0.20.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1071 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/LICENSE
--rw-r--r--   0        0        0     2082 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/README.md
--rw-r--r--   0        0        0      289 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/__init__.pyi
--rw-r--r--   0        0        0      438 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/_test.pyi
--rw-r--r--   0        0        0     5050 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/auth.pyi
--rw-r--r--   0        0        0      128 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/checksums.pyi
--rw-r--r--   0        0        0       94 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/common.pyi
--rw-r--r--   0        0        0     1878 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/crypto.pyi
--rw-r--r--   0        0        0     1707 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/eventstream/__init__.pyi
--rw-r--r--   0        0        0     3716 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/eventstream/rpc.pyi
--rw-r--r--   0        0        0      234 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/exceptions.pyi
--rw-r--r--   0        0        0     4713 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/http.pyi
--rw-r--r--   0        0        0     4723 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/io.pyi
--rw-r--r--   0        0        0     5007 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/mqtt.pyi
--rw-r--r--   0        0        0    13363 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/mqtt5.pyi
--rw-r--r--   0        0        0        0 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/py.typed
--rw-r--r--   0        0        0     5925 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/s3.pyi
--rw-r--r--   0        0        0     3414 2024-03-01 01:11:23.308223 types_awscrt-0.20.5/awscrt-stubs/websocket.pyi
--rw-r--r--   0        0        0     2549 2024-03-01 01:11:44.204337 types_awscrt-0.20.5/pyproject.toml
--rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 types_awscrt-0.20.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/LICENSE
+-rw-r--r--   0        0        0     2082 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/README.md
+-rw-r--r--   0        0        0      289 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/__init__.pyi
+-rw-r--r--   0        0        0      438 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/_test.pyi
+-rw-r--r--   0        0        0     5050 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/auth.pyi
+-rw-r--r--   0        0        0      128 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/checksums.pyi
+-rw-r--r--   0        0        0       94 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/common.pyi
+-rw-r--r--   0        0        0     1880 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/crypto.pyi
+-rw-r--r--   0        0        0     1707 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/eventstream/__init__.pyi
+-rw-r--r--   0        0        0     3716 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/eventstream/rpc.pyi
+-rw-r--r--   0        0        0      234 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     4713 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/http.pyi
+-rw-r--r--   0        0        0     4723 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/io.pyi
+-rw-r--r--   0        0        0     5007 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/mqtt.pyi
+-rw-r--r--   0        0        0    13365 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/mqtt5.pyi
+-rw-r--r--   0        0        0        0 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/py.typed
+-rw-r--r--   0        0        0     5925 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/s3.pyi
+-rw-r--r--   0        0        0     3414 2024-04-15 10:23:31.392300 types_awscrt-0.20.7/awscrt-stubs/websocket.pyi
+-rw-r--r--   0        0        0     2549 2024-04-15 10:23:53.540155 types_awscrt-0.20.7/pyproject.toml
+-rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 types_awscrt-0.20.7/PKG-INFO
```

### Comparing `types_awscrt-0.20.5/LICENSE` & `types_awscrt-0.20.7/LICENSE`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/README.md` & `types_awscrt-0.20.7/README.md`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/awscrt-stubs/auth.pyi` & `types_awscrt-0.20.7/awscrt-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/awscrt-stubs/crypto.pyi` & `types_awscrt-0.20.7/awscrt-stubs/crypto.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     PKCS1_5_SHA256: int
     PSS_SHA256: int
 
 class RSA(NativeResource):
     def __init__(self, binding: Any) -> None: ...
     @staticmethod
     def new_private_key_from_pem_data(
-        pem_data: Union[str, bytes, bytearray, memoryview]
+        pem_data: Union[str, bytes, bytearray, memoryview],
     ) -> "RSA": ...
     @staticmethod
     def new_public_key_from_pem_data(
-        pem_data: Union[str, bytes, bytearray, memoryview]
+        pem_data: Union[str, bytes, bytearray, memoryview],
     ) -> "RSA": ...
     def encrypt(
         self,
         encryption_algorithm: RSAEncryptionAlgorithm,
         plaintext: Union[bytes, bytearray, memoryview],
     ) -> bytes: ...
     def decrypt(
```

### Comparing `types_awscrt-0.20.5/awscrt-stubs/eventstream/__init__.pyi` & `types_awscrt-0.20.7/awscrt-stubs/eventstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/awscrt-stubs/eventstream/rpc.pyi` & `types_awscrt-0.20.7/awscrt-stubs/eventstream/rpc.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/awscrt-stubs/http.pyi` & `types_awscrt-0.20.7/awscrt-stubs/http.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/awscrt-stubs/io.pyi` & `types_awscrt-0.20.7/awscrt-stubs/io.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/awscrt-stubs/mqtt.pyi` & `types_awscrt-0.20.7/awscrt-stubs/mqtt.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/awscrt-stubs/mqtt5.pyi` & `types_awscrt-0.20.7/awscrt-stubs/mqtt5.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 class UnsubackReasonCode(IntEnum):
     SUCCESS: int
     NO_SUBSCRIPTION_EXISTED: int
     UNSPECIFIED_ERROR: int
     IMPLEMENTATION_SPECIFIC_ERROR: int
     NOT_AUTHORIZED: int
-    TOPIC_NAME_INVALID: int
+    TOPIC_FILTER_INVALID: int
     PACKET_IDENTIFIER_IN_USE: int
 
 class ClientSessionBehaviorType(IntEnum):
     DEFAULT: int
     CLEAN: int
     REJOIN_POST_SUCCESS: int
     REJOIN_ALWAYS: int
```

### Comparing `types_awscrt-0.20.5/awscrt-stubs/s3.pyi` & `types_awscrt-0.20.7/awscrt-stubs/s3.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/awscrt-stubs/websocket.pyi` & `types_awscrt-0.20.7/awscrt-stubs/websocket.pyi`

 * *Files identical despite different names*

### Comparing `types_awscrt-0.20.5/pyproject.toml` & `types_awscrt-0.20.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [tool.isort]
 profile = "black"
 line_length = 100
 src_paths = []
 
 [tool.poetry]
 name = "types-awscrt"
-version = "0.20.5"
+version = "0.20.7"
 description = "Type annotations and code completion for awscrt"
 authors = ["Vlad Emelianov <vlad.emelianov.nz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://youtype.github.io/mypy_boto3_builder/"
 repository = "https://github.com/youtype/types-awscrt"
 documentation = "https://youtype.github.io/mypy_boto3_builder/"
```

### Comparing `types_awscrt-0.20.5/PKG-INFO` & `types_awscrt-0.20.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-awscrt
-Version: 0.20.5
+Version: 0.20.7
 Summary: Type annotations and code completion for awscrt
 Home-page: https://youtype.github.io/mypy_boto3_builder/
 License: MIT
 Keywords: awscrt,type-annotations,pyright,mypy,boto3
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 Requires-Python: >=3.7,<4.0
```
