# Comparing `tmp/telegram_collector-0.2.7.tar.gz` & `tmp/telegram_collector-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.2.7.tar", last modified: Mon Apr 15 02:11:46 2024, max compression
+gzip compressed data, was "telegram_collector-0.2.8.tar", last modified: Mon Apr 15 02:16:09 2024, max compression
```

## Comparing `telegram_collector-0.2.7.tar` & `telegram_collector-0.2.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 02:11:46.304119 telegram_collector-0.2.7/
--rw-rw-rw-   0        0        0      317 2024-04-15 02:11:46.304119 telegram_collector-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-11 14:11:58.000000 telegram_collector-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 02:11:46.305118 telegram_collector-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      557 2024-04-15 02:11:44.000000 telegram_collector-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:11:46.294014 telegram_collector-0.2.7/telegram_collector/
--rw-rw-rw-   0        0        0     5297 2024-04-15 02:07:56.000000 telegram_collector-0.2.7/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0     1961 2024-04-11 14:22:26.000000 telegram_collector-0.2.7/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2542 2024-04-10 05:53:36.000000 telegram_collector-0.2.7/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:11:46.303138 telegram_collector-0.2.7/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      317 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 02:16:09.186114 telegram_collector-0.2.8/
+-rw-rw-rw-   0        0        0      317 2024-04-15 02:16:09.186114 telegram_collector-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-11 14:11:58.000000 telegram_collector-0.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 02:16:09.186114 telegram_collector-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      557 2024-04-15 02:16:07.000000 telegram_collector-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:16:09.177830 telegram_collector-0.2.8/telegram_collector/
+-rw-rw-rw-   0        0        0     5340 2024-04-15 02:16:07.000000 telegram_collector-0.2.8/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     1961 2024-04-11 14:22:26.000000 telegram_collector-0.2.8/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2821 2024-04-15 02:16:07.000000 telegram_collector-0.2.8/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:16:09.185130 telegram_collector-0.2.8/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      317 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-15 02:16:09.000000 telegram_collector-0.2.8/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.2.7/setup.py` & `telegram_collector-0.2.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.2.7',
+    version='0.2.8',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks', 'async_timeout'],
     entry_points={
```

### Comparing `telegram_collector-0.2.7/telegram_collector/__init__.py` & `telegram_collector-0.2.8/telegram_collector/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,36 +102,41 @@
         finally:
             await self.__terminate_client()
 
     async def __callback_send_message(self, event):
         try:
             message = event.message
             src_dialog_id = event.message.chat_id
-            print('get message',
-                  'time:', datetime.datetime.now().isoformat(),
-                  'chat_id:', src_dialog_id,
-                  'content:', message.text,
-                  'is_vid_or_pic:', message_is_video_or_photo(message))
+            print_message(message)
             if message_is_video_or_photo(message) and src_dialog_id in self.src_dialog_ids:
                 await self.__send_messages([message])
         except Exception as e:
             print('!!!ERROR!!!', e)
 
     # 流式汇总增量消息
     async def __send_new_message_src_to_dest(self):
-        self.client.add_event_handler(self.__callback_send_message, events.NewMessage(chats=self.src_dialogs, incoming=True))
+        self.client.add_event_handler(self.__callback_send_message,
+                                      events.NewMessage(chats=self.src_dialogs, incoming=True))
+        await self.__loop()
+
+    async def __loop(self):
         try:
-            while True:
-                # trigger
-                for i in self.src_dialogs():
-                    self.client.get_messages(i)
-                await asyncio.sleep(2)
+            await self.__trigger_get_message()
         finally:
             await self.__terminate_client()
 
+    async def __trigger_get_message(self):
+        while True:
+            # trigger
+            for i in self.src_dialogs():
+                messages = self.client.get_messages(i)
+                for message in messages:
+                    print_message(message)
+            await asyncio.sleep(2)
+
     async def __do_after_init(self, func):
         await self.__do_init()
         if asyncio.iscoroutinefunction(func):
             await func()
         else:
             func()
```

### Comparing `telegram_collector-0.2.7/telegram_collector/__main__.py` & `telegram_collector-0.2.8/telegram_collector/__main__.py`

 * *Files identical despite different names*

### Comparing `telegram_collector-0.2.7/telegram_collector/util.py` & `telegram_collector-0.2.8/telegram_collector/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import datetime
+
+
 def default_key_func(e):
     return get_message_size(e)
 
 
 def unique_messages(messages, key_func=default_key_func):
     added_key_set = set()
 
@@ -41,14 +44,22 @@
 
 
 def print_dialogs(dialogs):
     for dialog in dialogs:
         print(dialog.id, dialog.title)
 
 
+def print_message(message):
+    print('get message',
+          'time:', datetime.datetime.now().isoformat(),
+          'chat_id:', message.chat_id,
+          'content:', message.text,
+          'is_vid_or_pic:', message_is_video_or_photo(message))
+
+
 def get_video_or_photo_message(messages):
     ret = []
     for message in messages:
         if message_is_video_or_photo(message):
             ret.append(message)
     return ret
```

