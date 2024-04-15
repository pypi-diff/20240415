# Comparing `tmp/mobio-license-sdk-1.0.8.tar.gz` & `tmp/mobio-license-sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-license-sdk-1.0.8.tar", last modified: Mon Jun 28 04:01:01 2021, max compression
+gzip compressed data, was "mobio-license-sdk-1.0.9.tar", last modified: Mon Jun 28 08:13:06 2021, max compression
```

## Comparing `mobio-license-sdk-1.0.8.tar` & `mobio-license-sdk-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 04:01:01.674982 mobio-license-sdk-1.0.8/
--rw-rw-r--   0 theanh    (1000) theanh    (1000)     5111 2021-06-28 04:01:01.674982 mobio-license-sdk-1.0.8/PKG-INFO
--rw-r--r--   0 theanh    (1000) theanh    (1000)     4273 2021-06-28 03:58:56.000000 mobio-license-sdk-1.0.8/README.md
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 04:01:01.670983 mobio-license-sdk-1.0.8/mobio/
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 04:01:01.670983 mobio-license-sdk-1.0.8/mobio/sdks/
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 04:01:01.674982 mobio-license-sdk-1.0.8/mobio/sdks/license/
--rw-r--r--   0 theanh    (1000) theanh    (1000)      255 2021-06-28 03:58:56.000000 mobio-license-sdk-1.0.8/mobio/sdks/license/__init__.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     1988 2021-06-25 09:17:54.000000 mobio-license-sdk-1.0.8/mobio/sdks/license/config.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)    11103 2021-06-25 09:17:54.000000 mobio-license-sdk-1.0.8/mobio/sdks/license/crypt_utils.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     2535 2021-06-25 09:17:54.000000 mobio-license-sdk-1.0.8/mobio/sdks/license/license_detail_mess_used.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     1313 2021-06-14 07:31:46.000000 mobio-license-sdk-1.0.8/mobio/sdks/license/license_history_mess_used.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     2475 2021-06-14 07:31:46.000000 mobio-license-sdk-1.0.8/mobio/sdks/license/license_mess_used.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)     6664 2021-06-28 03:58:56.000000 mobio-license-sdk-1.0.8/mobio/sdks/license/license_sdk.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)      841 2021-06-14 07:31:46.000000 mobio-license-sdk-1.0.8/mobio/sdks/license/mongo_connection.py
--rw-r--r--   0 theanh    (1000) theanh    (1000)    33680 2021-06-28 03:58:56.000000 mobio-license-sdk-1.0.8/mobio/sdks/license/utils.py
-drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 04:01:01.674982 mobio-license-sdk-1.0.8/mobio_license_sdk.egg-info/
--rw-rw-r--   0 theanh    (1000) theanh    (1000)     5111 2021-06-28 04:01:01.000000 mobio-license-sdk-1.0.8/mobio_license_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 theanh    (1000) theanh    (1000)      617 2021-06-28 04:01:01.000000 mobio-license-sdk-1.0.8/mobio_license_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 theanh    (1000) theanh    (1000)        1 2021-06-28 04:01:01.000000 mobio-license-sdk-1.0.8/mobio_license_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 theanh    (1000) theanh    (1000)        6 2021-06-28 04:01:01.000000 mobio-license-sdk-1.0.8/mobio_license_sdk.egg-info/namespace_packages.txt
--rw-rw-r--   0 theanh    (1000) theanh    (1000)      132 2021-06-28 04:01:01.000000 mobio-license-sdk-1.0.8/mobio_license_sdk.egg-info/requires.txt
--rw-rw-r--   0 theanh    (1000) theanh    (1000)        6 2021-06-28 04:01:01.000000 mobio-license-sdk-1.0.8/mobio_license_sdk.egg-info/top_level.txt
--rw-r--r--   0 theanh    (1000) theanh    (1000)      104 2021-06-14 07:31:46.000000 mobio-license-sdk-1.0.8/pyproject.toml
--rw-rw-r--   0 theanh    (1000) theanh    (1000)       38 2021-06-28 04:01:01.674982 mobio-license-sdk-1.0.8/setup.cfg
--rw-r--r--   0 theanh    (1000) theanh    (1000)     9392 2021-06-28 04:00:35.000000 mobio-license-sdk-1.0.8/setup.py
+drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 08:13:06.624556 mobio-license-sdk-1.0.9/
+-rw-rw-r--   0 theanh    (1000) theanh    (1000)     5181 2021-06-28 08:13:06.624556 mobio-license-sdk-1.0.9/PKG-INFO
+-rw-r--r--   0 theanh    (1000) theanh    (1000)     4343 2021-06-28 08:12:51.000000 mobio-license-sdk-1.0.9/README.md
+drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 08:13:06.620556 mobio-license-sdk-1.0.9/mobio/
+drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 08:13:06.620556 mobio-license-sdk-1.0.9/mobio/sdks/
+drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 08:13:06.624556 mobio-license-sdk-1.0.9/mobio/sdks/license/
+-rw-r--r--   0 theanh    (1000) theanh    (1000)      255 2021-06-28 08:12:51.000000 mobio-license-sdk-1.0.9/mobio/sdks/license/__init__.py
+-rw-r--r--   0 theanh    (1000) theanh    (1000)     1988 2021-06-25 09:17:54.000000 mobio-license-sdk-1.0.9/mobio/sdks/license/config.py
+-rw-r--r--   0 theanh    (1000) theanh    (1000)    11829 2021-06-28 08:12:51.000000 mobio-license-sdk-1.0.9/mobio/sdks/license/crypt_utils.py
+-rw-r--r--   0 theanh    (1000) theanh    (1000)     2535 2021-06-25 09:17:54.000000 mobio-license-sdk-1.0.9/mobio/sdks/license/license_detail_mess_used.py
+-rw-r--r--   0 theanh    (1000) theanh    (1000)     1313 2021-06-14 07:31:46.000000 mobio-license-sdk-1.0.9/mobio/sdks/license/license_history_mess_used.py
+-rw-r--r--   0 theanh    (1000) theanh    (1000)     2475 2021-06-14 07:31:46.000000 mobio-license-sdk-1.0.9/mobio/sdks/license/license_mess_used.py
+-rw-r--r--   0 theanh    (1000) theanh    (1000)     6664 2021-06-28 03:58:56.000000 mobio-license-sdk-1.0.9/mobio/sdks/license/license_sdk.py
+-rw-r--r--   0 theanh    (1000) theanh    (1000)      841 2021-06-14 07:31:46.000000 mobio-license-sdk-1.0.9/mobio/sdks/license/mongo_connection.py
+-rw-r--r--   0 theanh    (1000) theanh    (1000)    33680 2021-06-28 03:58:56.000000 mobio-license-sdk-1.0.9/mobio/sdks/license/utils.py
+drwxrwxr-x   0 theanh    (1000) theanh    (1000)        0 2021-06-28 08:13:06.624556 mobio-license-sdk-1.0.9/mobio_license_sdk.egg-info/
+-rw-rw-r--   0 theanh    (1000) theanh    (1000)     5181 2021-06-28 08:13:06.000000 mobio-license-sdk-1.0.9/mobio_license_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 theanh    (1000) theanh    (1000)      617 2021-06-28 08:13:06.000000 mobio-license-sdk-1.0.9/mobio_license_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 theanh    (1000) theanh    (1000)        1 2021-06-28 08:13:06.000000 mobio-license-sdk-1.0.9/mobio_license_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 theanh    (1000) theanh    (1000)        6 2021-06-28 08:13:06.000000 mobio-license-sdk-1.0.9/mobio_license_sdk.egg-info/namespace_packages.txt
+-rw-rw-r--   0 theanh    (1000) theanh    (1000)      132 2021-06-28 08:13:06.000000 mobio-license-sdk-1.0.9/mobio_license_sdk.egg-info/requires.txt
+-rw-rw-r--   0 theanh    (1000) theanh    (1000)        6 2021-06-28 08:13:06.000000 mobio-license-sdk-1.0.9/mobio_license_sdk.egg-info/top_level.txt
+-rw-r--r--   0 theanh    (1000) theanh    (1000)      104 2021-06-14 07:31:46.000000 mobio-license-sdk-1.0.9/pyproject.toml
+-rw-rw-r--   0 theanh    (1000) theanh    (1000)       38 2021-06-28 08:13:06.624556 mobio-license-sdk-1.0.9/setup.cfg
+-rw-r--r--   0 theanh    (1000) theanh    (1000)     9392 2021-06-28 08:12:51.000000 mobio-license-sdk-1.0.9/setup.py
```

### Comparing `mobio-license-sdk-1.0.8/PKG-INFO` & `mobio-license-sdk-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-license-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio license SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,license
@@ -192,11 +192,14 @@
     - thêm cơ chế cache file license, tự động tải mới file sau 1 khoảng thời gian    
 
 #### Log - 1.0.7
     - export các hàm mã hóa và giải mã    
 
 #### Log - 1.0.8
     - Hàm kiểm tra merchant đã hết hạn chưa     
+
+#### Log - 1.0.9
+    - sửa lỗi lấy cache thông tin license  
     
-    
+
```

### Comparing `mobio-license-sdk-1.0.8/README.md` & `mobio-license-sdk-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -168,10 +168,13 @@
     - thêm cơ chế cache file license, tự động tải mới file sau 1 khoảng thời gian    
 
 #### Log - 1.0.7
     - export các hàm mã hóa và giải mã    
 
 #### Log - 1.0.8
     - Hàm kiểm tra merchant đã hết hạn chưa     
+
+#### Log - 1.0.9
+    - sửa lỗi lấy cache thông tin license  
     
-    
+
```

### Comparing `mobio-license-sdk-1.0.8/mobio/sdks/license/config.py` & `mobio-license-sdk-1.0.9/mobio/sdks/license/config.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-1.0.8/mobio/sdks/license/crypt_utils.py` & `mobio-license-sdk-1.0.9/mobio/sdks/license/crypt_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -187,14 +187,15 @@
 
     @staticmethod
     def get_file_path_license(merchant_id):
         license_file_name = hashlib.md5(bytes(merchant_id, "utf-8")).hexdigest()
         file_path = "{}/{}.{}".format(
             PathDir.PATH_DIR_LICENSE_FILE, license_file_name, "license"
         )
+        print("file path: %r", file_path)
         return file_path
 
     @staticmethod
     def get_content_from_file(file_path):
         content_file = None
         if not os.path.exists(file_path):
             return content_file
@@ -203,14 +204,15 @@
                 with open(file_path, "r") as fout:
                     content_file = fout.read()
                     fout.close()
                 break
             except IOError as ex:
                 print("license_sdk::get_content_from_file():message: %s" % ex)
                 time.sleep(0.1)
+        print("content file license: %r", content_file)
         return content_file
 
     @staticmethod
     def save_data_to_file(file_path, data):
         while True:
             try:
                 Path(os.path.dirname(os.path.abspath(file_path))).mkdir(
@@ -292,28 +294,40 @@
             print("license_sdk::get_file_license_from_admin():message: {}".format(ex))
         return license_encrypt
 
     @staticmethod
     def get_license_encrypt(merchant_id):
         license_encrypt = ""
         try:
-            license_encrypt = CryptUtil().license_merchant.getitem(merchant_id)
+            try:
+                license_encrypt = CryptUtil().license_merchant.getitem(merchant_id)
+            except Exception as ex:
+                print("license_sdk::get_license_encrypt():get cache none for key: {}".format(ex))
+            print("license_encrypt cache: {}".format(license_encrypt))
             if not license_encrypt:
+                print("license_encrypt no cache")
                 if Mobio.vm_type:
+                    print("server get license")
                     if Mobio.AUTO_RENEW_FILE_LICENSE and Mobio.AUTO_RENEW_FILE_LICENSE == "yes":
+                        print("renew file license")
                         license_encrypt = CryptUtil.get_file_license_from_license(merchant_id)
                         if license_encrypt:
+                            print("renew success")
                             file_path = CryptUtil.get_file_path_license(merchant_id)
                             CryptUtil.save_data_to_file(file_path, license_encrypt)
                     if not license_encrypt:
+                        print("get content file license")
                         file_path = CryptUtil.get_file_path_license(merchant_id)
                         license_encrypt = CryptUtil.get_content_from_file(file_path)
                 else:
+                    print("local get file license")
                     license_encrypt = CryptUtil.get_file_license_from_admin(merchant_id)
-                CryptUtil().license_merchant.set_item(merchant_id, license_encrypt)
+                if license_encrypt:
+                    print("save cache file license")
+                    CryptUtil().license_merchant.set_item(merchant_id, license_encrypt)
         except Exception as ex:
             print("license_sdk::get_license_encrypt():message: {}".format(ex))
         return license_encrypt
 
     @staticmethod
     def get_file_license_from_license(merchant_id):
         from .license_sdk import MobioLicenseSDK
@@ -341,9 +355,8 @@
 
     @staticmethod
     def encrypt_mobio_crypt2(data: str):
         return MobioCrypt2.e1(data)
 
     @staticmethod
     def decrypt_mobio_crypt2(data: str):
-        return MobioCrypt2.d1(data, "utf-8")
-
+        return MobioCrypt2.d1(data, "utf-8")
```

### Comparing `mobio-license-sdk-1.0.8/mobio/sdks/license/license_detail_mess_used.py` & `mobio-license-sdk-1.0.9/mobio/sdks/license/license_detail_mess_used.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-1.0.8/mobio/sdks/license/license_history_mess_used.py` & `mobio-license-sdk-1.0.9/mobio/sdks/license/license_history_mess_used.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-1.0.8/mobio/sdks/license/license_mess_used.py` & `mobio-license-sdk-1.0.9/mobio/sdks/license/license_mess_used.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-1.0.8/mobio/sdks/license/license_sdk.py` & `mobio-license-sdk-1.0.9/mobio/sdks/license/license_sdk.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-1.0.8/mobio/sdks/license/mongo_connection.py` & `mobio-license-sdk-1.0.9/mobio/sdks/license/mongo_connection.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-1.0.8/mobio/sdks/license/utils.py` & `mobio-license-sdk-1.0.9/mobio/sdks/license/utils.py`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-1.0.8/mobio_license_sdk.egg-info/PKG-INFO` & `mobio-license-sdk-1.0.9/mobio_license_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-license-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: Mobio license SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,license
@@ -192,11 +192,14 @@
     - thêm cơ chế cache file license, tự động tải mới file sau 1 khoảng thời gian    
 
 #### Log - 1.0.7
     - export các hàm mã hóa và giải mã    
 
 #### Log - 1.0.8
     - Hàm kiểm tra merchant đã hết hạn chưa     
+
+#### Log - 1.0.9
+    - sửa lỗi lấy cache thông tin license  
     
-    
+
```

### Comparing `mobio-license-sdk-1.0.8/mobio_license_sdk.egg-info/SOURCES.txt` & `mobio-license-sdk-1.0.9/mobio_license_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-license-sdk-1.0.8/setup.py` & `mobio-license-sdk-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         # with open(Requirements.__requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
 
-version = "1.0.8"
+version = "1.0.9"
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
     #
     # $ pip install sampleproject
     #
```

