# Comparing `tmp/yuankong-0.6.tar.gz` & `tmp/yuankong-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuankong-0.6.tar", last modified: Mon Apr  1 04:40:18 2024, max compression
+gzip compressed data, was "yuankong-0.7.tar", last modified: Mon Apr 15 09:00:17 2024, max compression
```

## Comparing `yuankong-0.6.tar` & `yuankong-0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 04:40:18.336632 yuankong-0.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 03:43:24.000000 yuankong-0.6/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-04-01 04:40:18.336632 yuankong-0.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-04-01 03:43:24.000000 yuankong-0.6/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-01 04:40:18.336632 yuankong-0.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      719 2024-04-01 03:43:24.000000 yuankong-0.6/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 04:40:18.332632 yuankong-0.6/yuankong/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2024-04-01 03:43:24.000000 yuankong-0.6/yuankong/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 04:40:18.336632 yuankong-0.6/yuankong/rpa/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 03:43:24.000000 yuankong-0.6/yuankong/rpa/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 04:40:18.336632 yuankong-0.6/yuankong/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      136 2024-04-01 03:43:24.000000 yuankong-0.6/yuankong/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2804 2024-04-01 03:43:24.000000 yuankong-0.6/yuankong/utils/bucket.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3490 2024-04-01 03:43:24.000000 yuankong-0.6/yuankong/utils/logManager.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 04:40:18.336632 yuankong-0.6/yuankong.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-04-01 04:40:18.000000 yuankong-0.6/yuankong.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      281 2024-04-01 04:40:18.000000 yuankong-0.6/yuankong.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-01 04:40:18.000000 yuankong-0.6/yuankong.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-01 04:40:18.000000 yuankong-0.6/yuankong.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 08:59:13.000000 yuankong-0.7/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-04-15 09:00:17.067022 yuankong-0.7/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-04-15 08:59:13.000000 yuankong-0.7/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-15 09:00:17.067022 yuankong-0.7/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      719 2024-04-15 09:00:13.000000 yuankong-0.7/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/yuankong/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2024-04-15 08:59:13.000000 yuankong-0.7/yuankong/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/yuankong/rpa/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 08:59:13.000000 yuankong-0.7/yuankong/rpa/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/yuankong/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      136 2024-04-15 08:59:13.000000 yuankong-0.7/yuankong/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2860 2024-04-15 08:59:56.000000 yuankong-0.7/yuankong/utils/bucket.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3490 2024-04-15 08:59:13.000000 yuankong-0.7/yuankong/utils/logManager.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:00:17.067022 yuankong-0.7/yuankong.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      418 2024-04-15 09:00:17.000000 yuankong-0.7/yuankong.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      281 2024-04-15 09:00:17.000000 yuankong-0.7/yuankong.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-15 09:00:17.000000 yuankong-0.7/yuankong.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-15 09:00:17.000000 yuankong-0.7/yuankong.egg-info/top_level.txt
```

### Comparing `yuankong-0.6/setup.py` & `yuankong-0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yuankong',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     description='Basic function of YuankongAI',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',  # 这使得README.md可以正确渲染
     author='ltq_yuankong',
     author_email='1539365976@qq.com',
     # url='http://60.205.141.203:3000/ningkp/MetaAgent/src/user_isolation',
```

### Comparing `yuankong-0.6/yuankong/utils/bucket.py` & `yuankong-0.7/yuankong/utils/bucket.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     directories.reverse()
     return directories
 
 
 class Bucket:
     def __init__(self, end_point, bucket_name):
         auth = oss2.ProviderAuth(EnvironmentVariableCredentialsProvider())
-        self.bucket = oss2.Bucket(auth, end_point, bucket_name)
-
+        self.bucket = oss2.Bucket(auth, end_point, bucket_name,connect_timeout=1000,session=oss2.Session(pool_size=10))
         if not self._bucket_exist():
             self.bucket.create_bucket()
 
     def _bucket_exist(self):
         try:
             self.bucket.get_bucket_info()
         except oss2.exceptions.NoSuchBucket:
@@ -93,8 +92,8 @@
 
     # bucket.mkdir('admin/test')
 
     # rsp = bucket.upload('admin/test/debug.xml', './debug.xml')
     # print(rsp)
 
     rsp = bucket.download('6136e19a7f624ea3b33c8d6b70e22dce/2fc5ee66526d453fbee6214dde70c979/milestone.log', './milestone.log')
-    print(rsp)
+    print(rsp)
```

### Comparing `yuankong-0.6/yuankong/utils/logManager.py` & `yuankong-0.7/yuankong/utils/logManager.py`

 * *Files identical despite different names*

