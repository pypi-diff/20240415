# Comparing `tmp/nhmail-1.0.3.tar.gz` & `tmp/nhmail-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhmail-1.0.3.tar", last modified: Wed Apr 10 01:50:30 2024, max compression
+gzip compressed data, was "nhmail-1.0.4.tar", last modified: Mon Apr 15 06:37:27 2024, max compression
```

## Comparing `nhmail-1.0.3.tar` & `nhmail-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-10 01:50:30.633634 nhmail-1.0.3/
--rw-r--r--   0 phamchuong   (501) staff       (20)     1062 2024-04-08 06:19:52.000000 nhmail-1.0.3/LICENSE
--rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-10 01:50:30.633408 nhmail-1.0.3/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1086 2024-04-08 08:02:58.000000 nhmail-1.0.3/README.md
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-10 01:50:30.632453 nhmail-1.0.3/nhmail/
--rw-r--r--   0 phamchuong   (501) staff       (20)     1658 2024-04-09 01:16:26.000000 nhmail-1.0.3/nhmail/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-04-08 07:26:40.000000 nhmail-1.0.3/nhmail/client.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      350 2024-04-08 07:54:41.000000 nhmail-1.0.3/nhmail/constants.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      492 2024-04-10 01:49:36.000000 nhmail-1.0.3/nhmail/validators.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-10 01:50:30.633171 nhmail-1.0.3/nhmail.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      252 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)        1 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)        7 2024-04-10 01:50:30.000000 nhmail-1.0.3/nhmail.egg-info/top_level.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-10 01:50:30.633683 nhmail-1.0.3/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      757 2024-04-10 01:50:25.000000 nhmail-1.0.3/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-15 06:37:27.617926 nhmail-1.0.4/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1062 2024-04-08 06:19:52.000000 nhmail-1.0.4/LICENSE
+-rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-15 06:37:27.617725 nhmail-1.0.4/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1086 2024-04-08 08:02:58.000000 nhmail-1.0.4/README.md
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-15 06:37:27.616623 nhmail-1.0.4/nhmail/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1595 2024-04-15 06:36:15.000000 nhmail-1.0.4/nhmail/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-04-08 07:26:40.000000 nhmail-1.0.4/nhmail/client.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      350 2024-04-08 07:54:41.000000 nhmail-1.0.4/nhmail/constants.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      544 2024-04-10 06:04:47.000000 nhmail-1.0.4/nhmail/validators.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-15 06:37:27.617524 nhmail-1.0.4/nhmail.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-15 06:37:27.000000 nhmail-1.0.4/nhmail.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      252 2024-04-15 06:37:27.000000 nhmail-1.0.4/nhmail.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)        1 2024-04-15 06:37:27.000000 nhmail-1.0.4/nhmail.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-15 06:37:27.000000 nhmail-1.0.4/nhmail.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)        7 2024-04-15 06:37:27.000000 nhmail-1.0.4/nhmail.egg-info/top_level.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-15 06:37:27.617972 nhmail-1.0.4/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      757 2024-04-15 06:36:24.000000 nhmail-1.0.4/setup.py
```

### Comparing `nhmail-1.0.3/LICENSE` & `nhmail-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nhmail-1.0.3/PKG-INFO` & `nhmail-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhmail
-Version: 1.0.3
+Version: 1.0.4
 Summary: email of nandh SDK for Python
 Home-page: https://github.com/ITNHL/nh-mail-sdk
 Author: it@nandhlogistics.vn
 Author-email: it@nandhlogistics.vn
 License: Version 1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `nhmail-1.0.3/README.md` & `nhmail-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nhmail-1.0.3/nhmail/__init__.py` & `nhmail-1.0.4/nhmail/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 HEADERS = {
     "Authorization": LAMBDA_AUTHEN,
     "Content-Type": "application/json",
 }
 
 
 class MailWrapSystem:
-    
     def __init__(self, **kwargs):
         self.body = kwargs.get("body")
 
     def send_verify_password(self):
         try:
             SendEmailSchema().load(self.body)
         except ValidationError as err:
@@ -36,22 +35,22 @@
             raise ValueError(err.messages)
         response = ServiceHttpClient(base_url=LAMBDA_URI).execute(
             method="post",
             uri=ENDPOINT_FOR_SEND_EMAIL,
             body=self.body,
             headers=HEADERS,
         )
-        return response.get("response").get("result")
+        return "success"
 
     def send_staff_confirm(self):
         try:
             SendEmailSchema().load(self.body)
         except ValidationError as err:
             raise ValueError(err.messages)
         response = ServiceHttpClient(base_url=LAMBDA_URI).execute(
             method="post",
             uri=ENDPOINT_FOR_SEND_EMAIL,
             body=self.body,
             headers=HEADERS,
         )
 
-        return response.get("response").get("result")
+        return "success"
```

### Comparing `nhmail-1.0.3/nhmail/client.py` & `nhmail-1.0.4/nhmail/client.py`

 * *Files identical despite different names*

### Comparing `nhmail-1.0.3/nhmail.egg-info/PKG-INFO` & `nhmail-1.0.4/nhmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhmail
-Version: 1.0.3
+Version: 1.0.4
 Summary: email of nandh SDK for Python
 Home-page: https://github.com/ITNHL/nh-mail-sdk
 Author: it@nandhlogistics.vn
 Author-email: it@nandhlogistics.vn
 License: Version 1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `nhmail-1.0.3/setup.py` & `nhmail-1.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PKG = "nhmail"
-version = "1.0.3"
+version = "1.0.4"
 long_desc = (
     """This SDK is a programatic inteface into the mail APIs of NandH Logistics."""
 )
 
 setup(
     name=PKG,
     version=version,
```

