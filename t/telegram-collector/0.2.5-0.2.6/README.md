# Comparing `tmp/telegram_collector-0.2.5.tar.gz` & `tmp/telegram_collector-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.2.5.tar", last modified: Sun Apr 14 15:57:40 2024, max compression
+gzip compressed data, was "telegram_collector-0.2.6.tar", last modified: Sun Apr 14 16:11:36 2024, max compression
```

## Comparing `telegram_collector-0.2.5.tar` & `telegram_collector-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 15:57:40.925707 telegram_collector-0.2.5/
--rw-rw-rw-   0        0        0      317 2024-04-14 15:57:40.921055 telegram_collector-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-11 14:11:58.000000 telegram_collector-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 15:57:40.925707 telegram_collector-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      557 2024-04-14 15:57:36.000000 telegram_collector-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:57:40.904749 telegram_collector-0.2.5/telegram_collector/
--rw-rw-rw-   0        0        0     5154 2024-04-14 15:57:36.000000 telegram_collector-0.2.5/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0     1961 2024-04-11 14:22:26.000000 telegram_collector-0.2.5/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2542 2024-04-10 05:53:36.000000 telegram_collector-0.2.5/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:57:40.919055 telegram_collector-0.2.5/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      317 2024-04-14 15:57:40.000000 telegram_collector-0.2.5/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-14 15:57:40.000000 telegram_collector-0.2.5/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 15:57:40.000000 telegram_collector-0.2.5/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-14 15:57:40.000000 telegram_collector-0.2.5/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-04-14 15:57:40.000000 telegram_collector-0.2.5/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-14 15:57:40.000000 telegram_collector-0.2.5/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 16:11:36.153153 telegram_collector-0.2.6/
+-rw-rw-rw-   0        0        0      317 2024-04-14 16:11:36.149616 telegram_collector-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-11 14:11:58.000000 telegram_collector-0.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-14 16:11:36.154154 telegram_collector-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      557 2024-04-14 16:11:26.000000 telegram_collector-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 16:11:36.131609 telegram_collector-0.2.6/telegram_collector/
+-rw-rw-rw-   0        0        0     5178 2024-04-14 16:11:26.000000 telegram_collector-0.2.6/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     1961 2024-04-11 14:22:26.000000 telegram_collector-0.2.6/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2542 2024-04-10 05:53:36.000000 telegram_collector-0.2.6/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-14 16:11:36.144322 telegram_collector-0.2.6/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      317 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.2.5/setup.py` & `telegram_collector-0.2.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.2.5',
+    version='0.2.6',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks', 'async_timeout'],
     entry_points={
```

### Comparing `telegram_collector-0.2.5/telegram_collector/__init__.py` & `telegram_collector-0.2.6/telegram_collector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             if message_is_video_or_photo(message) and src_dialog_id in self.src_dialog_ids:
                 await self.__send_messages([message])
         except Exception as e:
             print('!!!ERROR!!!', e)
 
     # 流式汇总增量消息
     async def __send_new_message_src_to_dest(self):
-        self.client.add_event_handler(self.__callback_send_message, events.NewMessage(incoming=True))
+        self.client.add_event_handler(self.__callback_send_message, events.NewMessage(chats=self.src_dialogs, incoming=True))
         try:
             while True:
                 await asyncio.sleep(1000)
         finally:
             await self.__terminate_client()
 
     async def __do_after_init(self, func):
```

### Comparing `telegram_collector-0.2.5/telegram_collector/__main__.py` & `telegram_collector-0.2.6/telegram_collector/__main__.py`

 * *Files identical despite different names*

### Comparing `telegram_collector-0.2.5/telegram_collector/util.py` & `telegram_collector-0.2.6/telegram_collector/util.py`

 * *Files identical despite different names*

