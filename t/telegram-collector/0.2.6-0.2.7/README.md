# Comparing `tmp/telegram_collector-0.2.6.tar.gz` & `tmp/telegram_collector-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.2.6.tar", last modified: Sun Apr 14 16:11:36 2024, max compression
+gzip compressed data, was "telegram_collector-0.2.7.tar", last modified: Mon Apr 15 02:11:46 2024, max compression
```

## Comparing `telegram_collector-0.2.6.tar` & `telegram_collector-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 16:11:36.153153 telegram_collector-0.2.6/
--rw-rw-rw-   0        0        0      317 2024-04-14 16:11:36.149616 telegram_collector-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-11 14:11:58.000000 telegram_collector-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 16:11:36.154154 telegram_collector-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      557 2024-04-14 16:11:26.000000 telegram_collector-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 16:11:36.131609 telegram_collector-0.2.6/telegram_collector/
--rw-rw-rw-   0        0        0     5178 2024-04-14 16:11:26.000000 telegram_collector-0.2.6/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0     1961 2024-04-11 14:22:26.000000 telegram_collector-0.2.6/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2542 2024-04-10 05:53:36.000000 telegram_collector-0.2.6/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-14 16:11:36.144322 telegram_collector-0.2.6/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      317 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-14 16:11:36.000000 telegram_collector-0.2.6/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 02:11:46.304119 telegram_collector-0.2.7/
+-rw-rw-rw-   0        0        0      317 2024-04-15 02:11:46.304119 telegram_collector-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-11 14:11:58.000000 telegram_collector-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 02:11:46.305118 telegram_collector-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      557 2024-04-15 02:11:44.000000 telegram_collector-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:11:46.294014 telegram_collector-0.2.7/telegram_collector/
+-rw-rw-rw-   0        0        0     5297 2024-04-15 02:07:56.000000 telegram_collector-0.2.7/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     1961 2024-04-11 14:22:26.000000 telegram_collector-0.2.7/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2542 2024-04-10 05:53:36.000000 telegram_collector-0.2.7/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:11:46.303138 telegram_collector-0.2.7/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      317 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-15 02:11:46.000000 telegram_collector-0.2.7/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.2.6/setup.py` & `telegram_collector-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.2.6',
+    version='0.2.7',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks', 'async_timeout'],
     entry_points={
```

### Comparing `telegram_collector-0.2.6/telegram_collector/__init__.py` & `telegram_collector-0.2.7/telegram_collector/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,18 @@
             print('!!!ERROR!!!', e)
 
     # 流式汇总增量消息
     async def __send_new_message_src_to_dest(self):
         self.client.add_event_handler(self.__callback_send_message, events.NewMessage(chats=self.src_dialogs, incoming=True))
         try:
             while True:
-                await asyncio.sleep(1000)
+                # trigger
+                for i in self.src_dialogs():
+                    self.client.get_messages(i)
+                await asyncio.sleep(2)
         finally:
             await self.__terminate_client()
 
     async def __do_after_init(self, func):
         await self.__do_init()
         if asyncio.iscoroutinefunction(func):
             await func()
```

### Comparing `telegram_collector-0.2.6/telegram_collector/__main__.py` & `telegram_collector-0.2.7/telegram_collector/__main__.py`

 * *Files identical despite different names*

### Comparing `telegram_collector-0.2.6/telegram_collector/util.py` & `telegram_collector-0.2.7/telegram_collector/util.py`

 * *Files identical despite different names*

