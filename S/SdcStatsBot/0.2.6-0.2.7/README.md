# Comparing `tmp/SdcStatsBot-0.2.6.tar.gz` & `tmp/sdcstatsbot-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SdcStatsBot-0.2.6.tar", last modified: Tue Apr  9 11:41:19 2024, max compression
+gzip compressed data, was "sdcstatsbot-0.2.7.tar", last modified: Mon Apr 15 16:54:38 2024, max compression
```

## Comparing `SdcStatsBot-0.2.6.tar` & `sdcstatsbot-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 11:41:19.390154 SdcStatsBot-0.2.6/
--rw-rw-rw-   0        0        0      344 2024-04-09 11:41:19.390154 SdcStatsBot-0.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 11:41:19.379610 SdcStatsBot-0.2.6/SDcStatsBot/
--rw-rw-rw-   0        0        0       26 2024-04-09 09:32:35.000000 SdcStatsBot-0.2.6/SDcStatsBot/__init__.py
--rw-rw-rw-   0        0        0     2271 2024-04-09 11:39:35.000000 SdcStatsBot-0.2.6/SDcStatsBot/client.py
-drwxrwxrwx   0        0        0        0 2024-04-09 11:41:19.389108 SdcStatsBot-0.2.6/SdcStatsBot.egg-info/
--rw-rw-rw-   0        0        0      344 2024-04-09 11:41:19.000000 SdcStatsBot-0.2.6/SdcStatsBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-09 11:41:19.000000 SdcStatsBot-0.2.6/SdcStatsBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 11:41:19.000000 SdcStatsBot-0.2.6/SdcStatsBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-09 11:41:19.000000 SdcStatsBot-0.2.6/SdcStatsBot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       23 2024-04-09 11:41:19.000000 SdcStatsBot-0.2.6/SdcStatsBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 11:41:19.000000 SdcStatsBot-0.2.6/SdcStatsBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 11:41:19.392367 SdcStatsBot-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      672 2024-04-09 11:41:00.000000 SdcStatsBot-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:54:38.386458 sdcstatsbot-0.2.7/
+-rw-rw-rw-   0        0        0      391 2024-04-15 16:54:38.386458 sdcstatsbot-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 16:54:38.375819 sdcstatsbot-0.2.7/SdcStatsBot/
+-rw-rw-rw-   0        0        0       26 2024-04-09 09:32:35.000000 sdcstatsbot-0.2.7/SdcStatsBot/__init__.py
+-rw-rw-rw-   0        0        0     2258 2024-04-09 11:43:52.000000 sdcstatsbot-0.2.7/SdcStatsBot/client.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:54:38.385952 sdcstatsbot-0.2.7/SdcStatsBot.egg-info/
+-rw-rw-rw-   0        0        0      391 2024-04-15 16:54:38.000000 sdcstatsbot-0.2.7/SdcStatsBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-15 16:54:38.000000 sdcstatsbot-0.2.7/SdcStatsBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 16:54:38.000000 sdcstatsbot-0.2.7/SdcStatsBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 16:54:38.000000 sdcstatsbot-0.2.7/SdcStatsBot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2024-04-15 16:54:38.000000 sdcstatsbot-0.2.7/SdcStatsBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 16:54:38.000000 sdcstatsbot-0.2.7/SdcStatsBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 16:54:38.388875 sdcstatsbot-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      647 2024-04-15 16:54:34.000000 sdcstatsbot-0.2.7/setup.py
```

### Comparing `SdcStatsBot-0.2.6/SDcStatsBot/client.py` & `sdcstatsbot-0.2.7/SdcStatsBot/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import aiohttp
 import asyncio
 
 class SdcApi:
-    def __init__(self, logger=None, interval=30):
+    def __init__(self, interval=30):
         if not isinstance(interval, int):
             raise ValueError("interval must be an integer")
         if interval < 30:
             raise ValueError("interval must be a positive integer")
 
         self.web_url = "https://api.server-discord.com/v2"
         self.session = aiohttp.ClientSession()
```

### Comparing `SdcStatsBot-0.2.6/setup.py` & `sdcstatsbot-0.2.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 setup(name='SdcStatsBot',
       author="Masezev",
       url="https://github.com/masezev/SdcStatsBot",
       project_urls={
           'Поддержка': 'https://discord.gg/H7FQFGEPz5',
       },
       repository='https://github.com/masezev/SdcStatsBot',
-      version='0.2.6',
+      version='0.2.7',
       description='A Python wrapper for the SDC API',
       python_requires='>=3.8.0',
       keywords='A Python wrapper for the SDC API',
       install_requires=[
             'aiohttp',
-            'loguru',
-            'logging',
+            'loguru'
       ],
-      packages=['SDcStatsBot'],
+      packages=['SdcStatsBot'],
       author_email='csgomanagement1@gmail.com',
       zip_safe=False)
```

