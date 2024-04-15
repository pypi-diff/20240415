# Comparing `tmp/dig_ass_chat_protos-0.0.7.tar.gz` & `tmp/dig_ass_chat_protos-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_chat_protos-0.0.7.tar", last modified: Fri Apr 12 21:04:10 2024, max compression
+gzip compressed data, was "dig_ass_chat_protos-0.0.8.tar", last modified: Mon Apr 15 13:09:54 2024, max compression
```

## Comparing `dig_ass_chat_protos-0.0.7.tar` & `dig_ass_chat_protos-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 21:04:10.317779 dig_ass_chat_protos-0.0.7/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.7/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 21:04:10.317779 dig_ass_chat_protos-0.0.7/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.7/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 21:04:10.317779 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2119 2024-04-12 21:04:09.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1273 2024-04-12 21:04:09.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3093 2024-04-12 21:04:09.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 21:03:26.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:20.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      871 2024-04-12 21:03:01.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 21:04:10.317779 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 21:04:10.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      533 2024-04-12 21:04:10.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 21:04:10.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 21:04:10.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-12 21:04:10.000000 dig_ass_chat_protos-0.0.7/dig_ass_chat_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.7/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 21:04:10.317779 dig_ass_chat_protos-0.0.7/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.7/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 13:09:54.926302 dig_ass_chat_protos-0.0.8/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.8/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-15 13:09:54.926302 dig_ass_chat_protos-0.0.8/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.8/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 13:09:54.926302 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2119 2024-04-15 13:09:53.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1273 2024-04-15 13:09:53.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3093 2024-04-15 13:09:53.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-15 13:01:41.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:20.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      997 2024-04-15 11:32:30.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 13:09:54.926302 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-15 13:09:54.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      533 2024-04-15 13:09:54.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-15 13:09:54.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-15 13:09:54.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-15 13:09:54.000000 dig_ass_chat_protos-0.0.8/dig_ass_chat_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.8/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-15 13:09:54.926302 dig_ass_chat_protos-0.0.8/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.8/setup.py
```

### Comparing `dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py` & `dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi` & `dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py` & `dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.7/dig_ass_chat_protos/client.py` & `dig_ass_chat_protos-0.0.8/dig_ass_chat_protos/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from google.protobuf.json_format import ParseDict
 from dig_ass_chat_protos.DigitalAssistantChatManager_pb2_grpc import DigitalAssistantChatManagerStub
 from dig_ass_chat_protos.DigitalAssistantChatManager_pb2 import DigitalAssistantChatManagerRequest, DigitalAssistantChatManagerResponse, OuterContextItem
 
 from .abstract_client import AbstractClient
 
 class ChatManagerClient(AbstractClient):
     def __init__(self, address) -> None:
         super().__init__(address)
         self._stub = DigitalAssistantChatManagerStub(self._channel)
 
     def __call__(self, text: str, outer_context: dict):
         request = DigitalAssistantChatManagerRequest(
             Text=text,
-            OuterContext=ParseDict(outer_context, OuterContextItem()),
+            OuterContext=OuterContextItem(
+                Sex=outer_context['Sex'],
+                Age=outer_context['Age'],
+                UserId=outer_context['UserId'],
+                SessionId=outer_context['SessionId']
+                ),
         )
         response: DigitalAssistantChatManagerResponse = self._stub.GetTextResponse(request)
         return response.Text
```

### Comparing `dig_ass_chat_protos-0.0.7/dig_ass_chat_protos.egg-info/SOURCES.txt` & `dig_ass_chat_protos-0.0.8/dig_ass_chat_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.7/setup.py` & `dig_ass_chat_protos-0.0.8/setup.py`

 * *Files identical despite different names*

