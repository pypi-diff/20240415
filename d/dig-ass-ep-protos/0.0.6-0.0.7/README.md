# Comparing `tmp/dig_ass_ep_protos-0.0.6.tar.gz` & `tmp/dig_ass_ep_protos-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ep_protos-0.0.6.tar", last modified: Fri Apr 12 21:04:22 2024, max compression
+gzip compressed data, was "dig_ass_ep_protos-0.0.7.tar", last modified: Mon Apr 15 13:09:42 2024, max compression
```

## Comparing `dig_ass_ep_protos-0.0.6.tar` & `dig_ass_ep_protos-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 21:04:22.305973 dig_ass_ep_protos-0.0.6/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-0.0.6/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-12 21:04:22.305973 dig_ass_ep_protos-0.0.6/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.6/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 21:04:22.305973 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2166 2024-04-12 21:04:20.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1455 2024-04-12 21:04:20.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-04-12 21:04:20.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 21:03:44.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      937 2024-04-12 21:03:37.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 21:04:22.305973 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-12 21:04:22.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      508 2024-04-12 21:04:22.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 21:04:22.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 21:04:22.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-04-12 21:04:22.000000 dig_ass_ep_protos-0.0.6/dig_ass_ep_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-0.0.6/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 21:04:22.305973 dig_ass_ep_protos-0.0.6/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-04-11 10:22:56.000000 dig_ass_ep_protos-0.0.6/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 13:09:42.126085 dig_ass_ep_protos-0.0.7/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-0.0.7/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-15 13:09:42.126085 dig_ass_ep_protos-0.0.7/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.7/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 13:09:42.126085 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2166 2024-04-15 13:09:40.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1455 2024-04-15 13:09:40.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-04-15 13:09:40.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-15 13:01:41.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1063 2024-04-15 11:32:29.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 13:09:42.126085 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-15 13:09:42.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      508 2024-04-15 13:09:42.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-15 13:09:42.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-15 13:09:42.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-04-15 13:09:42.000000 dig_ass_ep_protos-0.0.7/dig_ass_ep_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-0.0.7/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-15 13:09:42.126085 dig_ass_ep_protos-0.0.7/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-04-11 10:22:56.000000 dig_ass_ep_protos-0.0.7/setup.py
```

### Comparing `dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py` & `dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi` & `dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.6/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py` & `dig_ass_ep_protos-0.0.7/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.6/setup.py` & `dig_ass_ep_protos-0.0.7/setup.py`

 * *Files identical despite different names*

