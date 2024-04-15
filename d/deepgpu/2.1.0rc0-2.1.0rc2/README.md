# Comparing `tmp/deepgpu-2.1.0rc0.tar.gz` & `tmp/deepgpu-2.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgpu-2.1.0rc0.tar", last modified: Mon Nov 13 07:35:08 2023, max compression
+gzip compressed data, was "deepgpu-2.1.0rc2.tar", last modified: Mon Apr 15 03:31:24 2024, max compression
```

## Comparing `deepgpu-2.1.0rc0.tar` & `deepgpu-2.1.0rc2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 07:35:08.587759 deepgpu-2.1.0rc0/
--rw-r--r--   0 root         (0) root         (0)       30 2023-11-13 07:30:51.000000 deepgpu-2.1.0rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      615 2023-11-13 07:35:08.583878 deepgpu-2.1.0rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       62 2023-11-13 07:30:51.000000 deepgpu-2.1.0rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 07:35:08.514806 deepgpu-2.1.0rc0/deepgpu/
--rw-r--r--   0 root         (0) root         (0)       17 2023-11-13 07:30:15.000000 deepgpu-2.1.0rc0/deepgpu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-13 07:35:08.566927 deepgpu-2.1.0rc0/deepgpu.egg-info/
--rw-r--r--   0 root         (0) root         (0)      615 2023-11-13 07:35:08.000000 deepgpu-2.1.0rc0/deepgpu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      196 2023-11-13 07:35:08.000000 deepgpu-2.1.0rc0/deepgpu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-13 07:35:08.000000 deepgpu-2.1.0rc0/deepgpu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-11-13 07:35:08.000000 deepgpu-2.1.0rc0/deepgpu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-13 07:35:08.590110 deepgpu-2.1.0rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7329 2023-11-13 07:33:41.000000 deepgpu-2.1.0rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:31:24.255031 deepgpu-2.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)       30 2024-03-15 02:47:11.000000 deepgpu-2.1.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-15 03:31:24.241978 deepgpu-2.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      292 2024-04-15 01:48:58.000000 deepgpu-2.1.0rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:31:24.145225 deepgpu-2.1.0rc2/deepgpu/
+-rw-r--r--   0 root         (0) root         (0)       17 2024-03-15 02:47:11.000000 deepgpu-2.1.0rc2/deepgpu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 03:31:24.222051 deepgpu-2.1.0rc2/deepgpu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-15 03:31:23.000000 deepgpu-2.1.0rc2/deepgpu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      196 2024-04-15 03:31:24.000000 deepgpu-2.1.0rc2/deepgpu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 03:31:23.000000 deepgpu-2.1.0rc2/deepgpu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-15 03:31:23.000000 deepgpu-2.1.0rc2/deepgpu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 03:31:24.257985 deepgpu-2.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6624 2024-04-15 02:44:57.000000 deepgpu-2.1.0rc2/setup.py
```

### Comparing `deepgpu-2.1.0rc0/PKG-INFO` & `deepgpu-2.1.0rc2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgpu
-Version: 2.1.0rc0
+Version: 2.1.0rc2
 Summary: DEEPGPU is a toolset for AI training acceleration on Alibaba Cloud.
 Home-page: https://www.aliyun.com
 Author: Alibaba Cloud
 License: Copyright (C) Alibaba Group Holding Limited
 Keywords: Distributed,Deep Learning,Communication,NCCL,Pytorch,Tensorflow
 Requires-Python: >=3.8
```

### Comparing `deepgpu-2.1.0rc0/deepgpu.egg-info/PKG-INFO` & `deepgpu-2.1.0rc2/deepgpu.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgpu
-Version: 2.1.0rc0
+Version: 2.1.0rc2
 Summary: DEEPGPU is a toolset for AI training acceleration on Alibaba Cloud.
 Home-page: https://www.aliyun.com
 Author: Alibaba Cloud
 License: Copyright (C) Alibaba Group Holding Limited
 Keywords: Distributed,Deep Learning,Communication,NCCL,Pytorch,Tensorflow
 Requires-Python: >=3.8
```

