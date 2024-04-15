# Comparing `tmp/wansuite-2.5.tar.gz` & `tmp/wansuite-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wansuite-2.5.tar", last modified: Sat Apr 13 12:40:59 2024, max compression
+gzip compressed data, was "dist\wansuite-3.0.tar", last modified: Mon Apr 15 11:25:12 2024, max compression
```

## Comparing `wansuite-2.5.tar` & `wansuite-3.0.tar`

### file list

```diff
@@ -1,16 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 12:40:59.000000 wansuite-2.5/
--rw-rw-rw-   0        0        0      213 2024-04-13 12:40:59.000000 wansuite-2.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-13 12:40:59.000000 wansuite-2.5/setup.cfg
--rw-rw-rw-   0        0        0      155 2024-04-13 12:40:33.000000 wansuite-2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 12:40:59.000000 wansuite-2.5/wansuite/
--rw-rw-rw-   0        0        0       84 2024-04-13 12:36:27.000000 wansuite-2.5/wansuite/__init__.py
--rw-rw-rw-   0        0        0    13166 2023-04-03 00:00:42.000000 wansuite-2.5/wansuite/investing.py
--rw-rw-rw-   0        0        0       89 2023-02-10 12:37:51.000000 wansuite-2.5/wansuite/iofile.py
--rw-rw-rw-   0        0        0     3659 2024-03-07 16:43:29.000000 wansuite-2.5/wansuite/msql.py
--rw-rw-rw-   0        0        0      145 2024-03-08 01:38:27.000000 wansuite-2.5/wansuite/sys.py
--rw-rw-rw-   0        0        0      397 2023-02-08 13:29:16.000000 wansuite-2.5/wansuite/wtime.py
-drwxrwxrwx   0        0        0        0 2024-04-13 12:40:59.000000 wansuite-2.5/wansuite.egg-info/
--rw-rw-rw-   0        0        0      213 2024-04-13 12:40:59.000000 wansuite-2.5/wansuite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-04-13 12:40:59.000000 wansuite-2.5/wansuite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 12:40:59.000000 wansuite-2.5/wansuite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-13 12:40:59.000000 wansuite-2.5/wansuite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 11:25:12.000000 wansuite-3.0/
+-rw-rw-rw-   0        0        0      213 2024-04-15 11:25:12.000000 wansuite-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:25:12.000000 wansuite-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      403 2024-04-15 11:24:57.000000 wansuite-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite/
+-rw-rw-rw-   0        0        0      102 2024-04-13 14:15:03.000000 wansuite-3.0/wansuite/__init__.py
+-rw-rw-rw-   0        0        0    13166 2023-04-03 00:00:42.000000 wansuite-3.0/wansuite/investing.py
+-rw-rw-rw-   0        0        0       89 2023-02-10 12:37:51.000000 wansuite-3.0/wansuite/iofile.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite/macrodata/
+-rw-rw-rw-   0        0        0       30 2024-04-13 11:06:09.000000 wansuite-3.0/wansuite/macrodata/__init__.py
+-rw-rw-rw-   0        0        0     7979 2024-03-15 09:32:37.000000 wansuite-3.0/wansuite/macrodata/updatefromfile.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite/marketdata/
+-rw-rw-rw-   0        0        0       30 2024-04-13 11:06:40.000000 wansuite-3.0/wansuite/marketdata/__init__.py
+-rw-rw-rw-   0        0        0    10788 2024-04-08 01:56:37.000000 wansuite-3.0/wansuite/marketdata/updateMarketData.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite/media/
+-rw-rw-rw-   0        0        0      247 2024-03-31 04:27:38.000000 wansuite-3.0/wansuite/media/__init__.py
+-rw-rw-rw-   0        0        0     2259 2024-03-11 04:23:20.000000 wansuite-3.0/wansuite/media/datacollection.py
+-rw-rw-rw-   0        0        0      927 2024-03-10 04:22:20.000000 wansuite-3.0/wansuite/media/datavis.py
+-rw-rw-rw-   0        0        0        0 2024-03-10 01:20:48.000000 wansuite-3.0/wansuite/media/network.py
+-rw-rw-rw-   0        0        0     4625 2024-04-01 00:06:35.000000 wansuite-3.0/wansuite/media/nownews.py
+-rw-rw-rw-   0        0        0        0 2024-03-10 01:19:33.000000 wansuite-3.0/wansuite/media/sentiment.py
+-rw-rw-rw-   0        0        0      284 2024-03-09 23:27:15.000000 wansuite-3.0/wansuite/media/sys.py
+-rw-rw-rw-   0        0        0     2508 2024-03-10 23:57:19.000000 wansuite-3.0/wansuite/media/textfeature.py
+-rw-rw-rw-   0        0        0     2765 2024-03-10 23:27:24.000000 wansuite-3.0/wansuite/media/textprocessing.py
+-rw-rw-rw-   0        0        0      512 2024-03-10 01:50:26.000000 wansuite-3.0/wansuite/media/topicmodel.py
+-rw-rw-rw-   0        0        0     3659 2024-03-07 16:43:29.000000 wansuite-3.0/wansuite/msql.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite/order/
+-rw-rw-rw-   0        0        0        0 2024-03-08 01:36:18.000000 wansuite-3.0/wansuite/order/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite/strategy/
+-rw-rw-rw-   0        0        0       18 2024-04-13 11:07:03.000000 wansuite-3.0/wansuite/strategy/__init__.py
+-rw-rw-rw-   0        0        0    21210 2024-03-25 13:03:06.000000 wansuite-3.0/wansuite/strategy/zack.py
+-rw-rw-rw-   0        0        0      122 2024-04-15 11:23:57.000000 wansuite-3.0/wansuite/sys.py
+-rw-rw-rw-   0        0        0      397 2023-02-08 13:29:16.000000 wansuite-3.0/wansuite/wtime.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 11:25:12.000000 wansuite-3.0/wansuite.egg-info/top_level.txt
```

### Comparing `wansuite-2.5/wansuite/investing.py` & `wansuite-3.0/wansuite/investing.py`

 * *Files identical despite different names*

### Comparing `wansuite-2.5/wansuite/msql.py` & `wansuite-3.0/wansuite/msql.py`

 * *Files identical despite different names*

