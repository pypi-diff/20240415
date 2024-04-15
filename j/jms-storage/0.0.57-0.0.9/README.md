# Comparing `tmp/jms-storage-0.0.57.tar.gz` & `tmp/jms-storage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jms-storage-0.0.57.tar", last modified: Mon Apr 15 06:26:53 2024, max compression
+gzip compressed data, was "dist/jms-storage-0.0.9.tar", last modified: Thu Mar  8 16:18:39 2018, max compression
```

## Comparing `jms-storage-0.0.57.tar` & `jms-storage-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:26:53.258561 jms-storage-0.0.57/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-15 06:26:53.258561 jms-storage-0.0.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 06:26:45.000000 jms-storage-0.0.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:26:53.258561 jms-storage-0.0.57/jms_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/ceph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/es.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/jms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/obs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/oss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/sftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-15 06:26:45.000000 jms-storage-0.0.57/jms_storage/storage_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 06:26:53.258561 jms-storage-0.0.57/jms_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-15 06:26:53.000000 jms-storage-0.0.57/jms_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-15 06:26:53.000000 jms-storage-0.0.57/jms_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 06:26:53.000000 jms-storage-0.0.57/jms_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-15 06:26:53.000000 jms-storage-0.0.57/jms_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 06:26:53.000000 jms-storage-0.0.57/jms_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-15 06:26:45.000000 jms-storage-0.0.57/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 06:26:53.258561 jms-storage-0.0.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-15 06:26:45.000000 jms-storage-0.0.57/setup.py
+drwxr-xr-x   0 liuzheng   (501) staff       (20)        0 2018-03-08 16:18:39.000000 jms-storage-0.0.9/
+-rw-r--r--   0 liuzheng   (501) staff       (20)      354 2018-03-08 16:18:39.000000 jms-storage-0.0.9/PKG-INFO
+drwxr-xr-x   0 liuzheng   (501) staff       (20)        0 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/
+-rw-r--r--   0 liuzheng   (501) staff       (20)      354 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/PKG-INFO
+-rw-r--r--   0 liuzheng   (501) staff       (20)      302 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 liuzheng   (501) staff       (20)      213 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/requires.txt
+-rw-r--r--   0 liuzheng   (501) staff       (20)       12 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/top_level.txt
+-rw-r--r--   0 liuzheng   (501) staff       (20)        1 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 liuzheng   (501) staff       (20)       25 2018-03-08 10:08:10.000000 jms-storage-0.0.9/README.md
+-rw-r--r--   0 liuzheng   (501) staff       (20)     1111 2018-03-08 14:51:32.000000 jms-storage-0.0.9/setup.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)       38 2018-03-08 16:18:39.000000 jms-storage-0.0.9/setup.cfg
+drwxr-xr-x   0 liuzheng   (501) staff       (20)        0 2018-03-08 16:18:39.000000 jms-storage-0.0.9/jms_storage/
+-rw-r--r--   0 liuzheng   (501) staff       (20)     4078 2018-01-23 10:44:05.000000 jms-storage-0.0.9/jms_storage/elasticsearch.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)     1172 2018-03-08 16:05:21.000000 jms-storage-0.0.9/jms_storage/ali.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)      372 2018-03-08 16:18:23.000000 jms-storage-0.0.9/jms_storage/__init__.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)     1674 2018-03-08 16:05:21.000000 jms-storage-0.0.9/jms_storage/aws.py
+-rw-r--r--   0 liuzheng   (501) staff       (20)      636 2018-03-08 16:05:21.000000 jms-storage-0.0.9/jms_storage/jms.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `jms-storage-0.0.57/jms_storage/azure.py` & `jms-storage-0.0.9/jms_storage/aws.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,52 @@
 # -*- coding: utf-8 -*-
 #
+import boto3
 
-import os
-
-from azure.storage.blob import BlobServiceClient
-
-from .base import ObjectStorage
-
-
-class AzureStorage(ObjectStorage):
 
+class aws:
     def __init__(self, config):
-        self.account_name = config.get("ACCOUNT_NAME", None)
-        self.account_key = config.get("ACCOUNT_KEY", None)
-        self.container_name = config.get("CONTAINER_NAME", None)
-        self.endpoint_suffix = config.get("ENDPOINT_SUFFIX", 'core.chinacloudapi.cn')
-
-        if self.account_name and self.account_key:
-            self.service_client = BlobServiceClient(
-                account_url=f'https://{self.account_name}.blob.{self.endpoint_suffix}',
-                credential={'account_name': self.account_name, 'account_key': self.account_key}
-            )
-            self.client = self.service_client.get_container_client(self.container_name)
+        self.BUCKET = config.get("BUCKET", "jumpserver")
+        self.REGION = config.get("REGION", None)
+        self.ACCESS_KEY = config.get("ACCESS_KEY", None)
+        self.SECRET_KEY = config.get("SECRET_KEY", None)
+        if self.ACCESS_KEY and self.REGION and self.SECRET_KEY:
+            self.client = boto3.client('s3',
+                                        region_name=self.REGION,
+                                        aws_access_key_id=self.ACCESS_KEY,
+                                        aws_secret_access_key=self.SECRET_KEY)
         else:
-            self.client = None
+            self.client = boto3.client('s3')
 
-    def upload(self, src, target):
-        try:
-            self.client.upload_blob(target, src)
-            return True, None
-        except Exception as e:
-            return False, e
+    def type(self):
+        return 's3'
 
-    def download(self, src, target):
+    def upload_file(self, filepath, remote_path):
         try:
-            blob_data = self.client.download_blob(blob=src)
-            os.makedirs(os.path.dirname(target), 0o755, exist_ok=True)
-            with open(target, 'wb') as writer:
-                writer.write(blob_data.readall())
-            return True, None
-        except Exception as e:
-            return False, e
+            self.client.upload_file(filepath, self.BUCKET, remote_path)
+            return True
+        except:
+            return False
 
-    def delete(self, path):
+    def check_file(self, remote_path):
         try:
-            self.client.delete_blob(path)
-            return True, False
-        except Exception as e:
-            return False, e
-
-    def exists(self, path):
-        resp = self.client.list_blobs(name_starts_with=path)
-        return len(list(resp)) != 0
+            self.client.head_object(Bucket=self.BUCKET, Key=remote_path)
+            return True
+        except:
+            return False
 
-    def list_buckets(self):
-        return list(self.service_client.list_containers())
+    def download_file(self, remote_path, locale_path):
+        try:
+            self.client.download_file(self.BUCKET, remote_path, locale_path)
+            return True
+        except:
+            return False
 
-    @property
-    def type(self):
-        return 'azure'
+    def generate_presigned_url(self, path, expire=3600):
+        try:
+            return self.client.generate_presigned_url(
+                ClientMethod='get_object',
+                Params={'Bucket': self.BUCKET, 'Key': path},
+                ExpiresIn=expire,
+                HttpMethod='GET')
+        except:
+            return False
```

### Comparing `jms-storage-0.0.57/jms_storage/jms.py` & `jms-storage-0.0.9/jms_storage/ali.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 # -*- coding: utf-8 -*-
 #
-import os
-from .base import ObjectStorage, LogStorage
+import oss2
 
 
-class JMSReplayStorage(ObjectStorage):
+class ali:
     def __init__(self, config):
-        self.client = config.get("SERVICE")
+        self.ENDPOINT = config.get("ENDPOINT", None)
+        self.BUCKET = config.get("BUCKET", None)
+        self.ACCESS_KEY = config.get("ACCESS_KEY", None)
+        self.SECRET_KEY = config.get("SECRET_KEY", None)
+        if self.ACCESS_KEY and self.SECRET_KEY:
+            self.auth = oss2.Auth(self.ACCESS_KEY, self.SECRET_KEY)
+        else:
+            self.auth = None
+        if self.auth and self.ENDPOINT and self.BUCKET:
+            self.client = oss2.Bucket(self.auth, self.ENDPOINT, self.BUCKET)
+        else:
+            self.client = None
 
-    def upload(self, src, target):
-        session_id = os.path.basename(target).split('.')[0]
-        ok = self.client.push_session_replay(src, session_id)
-        return ok, None
-
-    def delete(self, path):
-        return False, Exception("Not support not")
-
-    def exists(self, path):
-        return False
-
-    def download(self, src, target):
-        return False, Exception("Not support not")
-
-    @property
     def type(self):
-        return 'jms'
-
+        return 'oss'
 
-class JMSCommandStorage(LogStorage):
-    def __init__(self, config):
-        self.client = config.get("SERVICE")
-        if not self.client:
-            raise Exception("Not found app service")
-
-    def save(self, command):
-        return self.client.push_session_command([command])
-
-    def bulk_save(self, command_set, raise_on_error=True):
-        return self.client.push_session_command(command_set)
-
-    def filter(self, date_from=None, date_to=None,
-               user=None, asset=None, account=None,
-               input=None, session=None):
-        pass
-
-    def count(self, date_from=None, date_to=None,
-              user=None, asset=None, account=None,
-              input=None, session=None):
-        pass
+    def upload_file(self, filepath, remote_path):
+        try:
+            self.client.put_object_from_file(remote_path, filepath)
+            return True
+        except:
+            return False
+
+    def check_file(self, remote_path):
+        return self.client.object_exists(remote_path)
+
+    def download_file(self, remote_path, locale_path):
+        try:
+            self.client.get_object_to_file(remote_path, locale_path)
+            return True
+        except:
+            return False
```

### Comparing `jms-storage-0.0.57/setup.py` & `jms-storage-0.0.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 #!/usr/bin/env python
 # coding: utf-8
 # Copyright (c) 2018
+# Gmail:liuzheng712
+#
+
+
 import re
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
@@ -14,35 +18,25 @@
 
 if not version:
     raise RuntimeError('Cannot find version information')
 
 with open('README.md', 'rb') as f:
     readme = f.read().decode('utf-8')
 
-with open('requirements.txt', 'r') as f:
-    requirements = [x.strip() for x in f.readlines()]
+with open('jms_storage.egg-info/requires.txt', 'r') as requirements_file:
+    requirements = [x.strip() for x in requirements_file.readlines()]
 
 setup(
     name='jms-storage',
     version=version,
-    keywords=['jumpserver', 'storage', 'oss', 's3', 'elasticsearch'],
+    keywords=['jumpserver', 'storage', 'oss', 's3', 'aws'],
     description='Jumpserver storage python sdk tools',
     long_description=readme,
     license='MIT Licence',
     url='http://www.jumpserver.org/',
     author='Jumpserver team',
-    author_email='support@fit2cloud.com',
+    author_email='liuzheng712@gmail.com',
     packages=['jms_storage'],
-    data_files=[('requirements', ['requirements.txt'])],
     include_package_data=True,
     install_requires=requirements,
     platforms='any',
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6'
-    ]
 )
```

