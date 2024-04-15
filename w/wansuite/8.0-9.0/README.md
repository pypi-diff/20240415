# Comparing `tmp/wansuite-8.0.tar.gz` & `tmp/wansuite-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wansuite-8.0.tar", last modified: Mon Apr 15 13:04:09 2024, max compression
+gzip compressed data, was "wansuite-9.0.tar", last modified: Mon Apr 15 13:12:21 2024, max compression
```

## Comparing `wansuite-8.0.tar` & `wansuite-9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.179399 wansuite-8.0/
--rw-r--r--   0 neuronpro   (501) staff       (20)       83 2024-04-15 13:04:09.179263 wansuite-8.0/PKG-INFO
--rw-r--r--   0 neuronpro   (501) staff       (20)       38 2024-04-15 13:04:09.179442 wansuite-8.0/setup.cfg
--rw-r--r--   0 neuronpro   (501) staff       (20)      468 2024-04-15 13:04:06.000000 wansuite-8.0/setup.py
-drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.176180 wansuite-8.0/wansuite/
--rw-r--r--   0 neuronpro   (501) staff       (20)      102 2024-04-13 14:15:03.000000 wansuite-8.0/wansuite/__init__.py
--rw-r--r--   0 neuronpro   (501) staff       (20)    13166 2023-04-03 00:00:42.000000 wansuite-8.0/wansuite/investing.py
--rw-r--r--   0 neuronpro   (501) staff       (20)       89 2023-02-10 12:37:51.000000 wansuite-8.0/wansuite/iofile.py
-drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.177120 wansuite-8.0/wansuite/macrodata/
--rw-r--r--   0 neuronpro   (501) staff       (20)       30 2024-04-13 11:06:09.000000 wansuite-8.0/wansuite/macrodata/__init__.py
--rw-r--r--   0 neuronpro   (501) staff       (20)     7979 2024-03-15 09:32:37.000000 wansuite-8.0/wansuite/macrodata/updatefromfile.py
-drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.177448 wansuite-8.0/wansuite/marketdata/
--rw-r--r--   0 neuronpro   (501) staff       (20)       30 2024-04-13 11:06:40.000000 wansuite-8.0/wansuite/marketdata/__init__.py
--rw-r--r--   0 neuronpro   (501) staff       (20)    10788 2024-04-08 01:56:37.000000 wansuite-8.0/wansuite/marketdata/updateMarketData.py
-drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.178719 wansuite-8.0/wansuite/media/
--rw-r--r--   0 neuronpro   (501) staff       (20)      247 2024-03-31 04:27:38.000000 wansuite-8.0/wansuite/media/__init__.py
--rw-r--r--   0 neuronpro   (501) staff       (20)     2259 2024-03-11 04:23:20.000000 wansuite-8.0/wansuite/media/datacollection.py
--rw-r--r--   0 neuronpro   (501) staff       (20)      927 2024-03-10 04:22:20.000000 wansuite-8.0/wansuite/media/datavis.py
--rw-r--r--   0 neuronpro   (501) staff       (20)        0 2024-03-10 01:20:48.000000 wansuite-8.0/wansuite/media/network.py
--rw-r--r--   0 neuronpro   (501) staff       (20)     4625 2024-04-01 00:06:35.000000 wansuite-8.0/wansuite/media/nownews.py
--rw-r--r--   0 neuronpro   (501) staff       (20)        0 2024-03-10 01:19:33.000000 wansuite-8.0/wansuite/media/sentiment.py
--rw-r--r--   0 neuronpro   (501) staff       (20)      284 2024-03-09 23:27:15.000000 wansuite-8.0/wansuite/media/sys.py
--rw-r--r--   0 neuronpro   (501) staff       (20)     2508 2024-03-10 23:57:19.000000 wansuite-8.0/wansuite/media/textfeature.py
--rw-r--r--   0 neuronpro   (501) staff       (20)     2765 2024-03-10 23:27:24.000000 wansuite-8.0/wansuite/media/textprocessing.py
--rw-r--r--   0 neuronpro   (501) staff       (20)      512 2024-03-10 01:50:26.000000 wansuite-8.0/wansuite/media/topicmodel.py
--rw-r--r--   0 neuronpro   (501) staff       (20)     3659 2024-03-07 16:43:29.000000 wansuite-8.0/wansuite/msql.py
-drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.178844 wansuite-8.0/wansuite/order/
--rw-r--r--   0 neuronpro   (501) staff       (20)        0 2024-03-08 01:36:18.000000 wansuite-8.0/wansuite/order/__init__.py
-drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.179061 wansuite-8.0/wansuite/strategy/
--rw-r--r--   0 neuronpro   (501) staff       (20)       18 2024-04-13 11:07:03.000000 wansuite-8.0/wansuite/strategy/__init__.py
--rw-r--r--   0 neuronpro   (501) staff       (20)    21210 2024-03-25 13:03:06.000000 wansuite-8.0/wansuite/strategy/zack.py
--rw-r--r--   0 neuronpro   (501) staff       (20)      122 2024-04-15 11:23:57.000000 wansuite-8.0/wansuite/sys.py
--rw-r--r--   0 neuronpro   (501) staff       (20)      397 2023-02-08 13:29:16.000000 wansuite-8.0/wansuite/wtime.py
-drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.176857 wansuite-8.0/wansuite.egg-info/
--rw-r--r--   0 neuronpro   (501) staff       (20)       83 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/PKG-INFO
--rw-r--r--   0 neuronpro   (501) staff       (20)      783 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/SOURCES.txt
--rw-r--r--   0 neuronpro   (501) staff       (20)        1 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/dependency_links.txt
--rw-r--r--   0 neuronpro   (501) staff       (20)      111 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/requires.txt
--rw-r--r--   0 neuronpro   (501) staff       (20)        9 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/top_level.txt
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:12:21.288694 wansuite-9.0/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       83 2024-04-15 13:12:21.288533 wansuite-9.0/PKG-INFO
+-rw-r--r--   0 neuronpro   (501) staff       (20)       38 2024-04-15 13:12:21.288745 wansuite-9.0/setup.cfg
+-rw-r--r--   0 neuronpro   (501) staff       (20)      441 2024-04-15 13:12:19.000000 wansuite-9.0/setup.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:12:21.284572 wansuite-9.0/wansuite/
+-rw-r--r--   0 neuronpro   (501) staff       (20)      102 2024-04-13 14:15:03.000000 wansuite-9.0/wansuite/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)    13166 2023-04-03 00:00:42.000000 wansuite-9.0/wansuite/investing.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)       89 2023-02-10 12:37:51.000000 wansuite-9.0/wansuite/iofile.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:12:21.285968 wansuite-9.0/wansuite/macrodata/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       30 2024-04-13 11:06:09.000000 wansuite-9.0/wansuite/macrodata/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     7979 2024-03-15 09:32:37.000000 wansuite-9.0/wansuite/macrodata/updatefromfile.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:12:21.286514 wansuite-9.0/wansuite/marketdata/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       30 2024-04-13 11:06:40.000000 wansuite-9.0/wansuite/marketdata/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)    10788 2024-04-08 01:56:37.000000 wansuite-9.0/wansuite/marketdata/updateMarketData.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:12:21.287919 wansuite-9.0/wansuite/media/
+-rw-r--r--   0 neuronpro   (501) staff       (20)      247 2024-03-31 04:27:38.000000 wansuite-9.0/wansuite/media/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     2259 2024-03-11 04:23:20.000000 wansuite-9.0/wansuite/media/datacollection.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      927 2024-03-10 04:22:20.000000 wansuite-9.0/wansuite/media/datavis.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)        0 2024-03-10 01:20:48.000000 wansuite-9.0/wansuite/media/network.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     4625 2024-04-01 00:06:35.000000 wansuite-9.0/wansuite/media/nownews.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)        0 2024-03-10 01:19:33.000000 wansuite-9.0/wansuite/media/sentiment.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      284 2024-03-09 23:27:15.000000 wansuite-9.0/wansuite/media/sys.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     2508 2024-03-10 23:57:19.000000 wansuite-9.0/wansuite/media/textfeature.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     2765 2024-03-10 23:27:24.000000 wansuite-9.0/wansuite/media/textprocessing.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      512 2024-03-10 01:50:26.000000 wansuite-9.0/wansuite/media/topicmodel.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     3659 2024-03-07 16:43:29.000000 wansuite-9.0/wansuite/msql.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:12:21.288051 wansuite-9.0/wansuite/order/
+-rw-r--r--   0 neuronpro   (501) staff       (20)        0 2024-03-08 01:36:18.000000 wansuite-9.0/wansuite/order/__init__.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:12:21.288276 wansuite-9.0/wansuite/strategy/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       18 2024-04-13 11:07:03.000000 wansuite-9.0/wansuite/strategy/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)    21210 2024-03-25 13:03:06.000000 wansuite-9.0/wansuite/strategy/zack.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      122 2024-04-15 11:23:57.000000 wansuite-9.0/wansuite/sys.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      397 2023-02-08 13:29:16.000000 wansuite-9.0/wansuite/wtime.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:12:21.285485 wansuite-9.0/wansuite.egg-info/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       83 2024-04-15 13:12:21.000000 wansuite-9.0/wansuite.egg-info/PKG-INFO
+-rw-r--r--   0 neuronpro   (501) staff       (20)      783 2024-04-15 13:12:21.000000 wansuite-9.0/wansuite.egg-info/SOURCES.txt
+-rw-r--r--   0 neuronpro   (501) staff       (20)        1 2024-04-15 13:12:21.000000 wansuite-9.0/wansuite.egg-info/dependency_links.txt
+-rw-r--r--   0 neuronpro   (501) staff       (20)       95 2024-04-15 13:12:21.000000 wansuite-9.0/wansuite.egg-info/requires.txt
+-rw-r--r--   0 neuronpro   (501) staff       (20)        9 2024-04-15 13:12:21.000000 wansuite-9.0/wansuite.egg-info/top_level.txt
```

### Comparing `wansuite-8.0/wansuite/investing.py` & `wansuite-9.0/wansuite/investing.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/macrodata/updatefromfile.py` & `wansuite-9.0/wansuite/macrodata/updatefromfile.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/marketdata/updateMarketData.py` & `wansuite-9.0/wansuite/marketdata/updateMarketData.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/media/datacollection.py` & `wansuite-9.0/wansuite/media/datacollection.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/media/datavis.py` & `wansuite-9.0/wansuite/media/datavis.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/media/nownews.py` & `wansuite-9.0/wansuite/media/nownews.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/media/textfeature.py` & `wansuite-9.0/wansuite/media/textfeature.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/media/textprocessing.py` & `wansuite-9.0/wansuite/media/textprocessing.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/media/topicmodel.py` & `wansuite-9.0/wansuite/media/topicmodel.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/msql.py` & `wansuite-9.0/wansuite/msql.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite/strategy/zack.py` & `wansuite-9.0/wansuite/strategy/zack.py`

 * *Files identical despite different names*

### Comparing `wansuite-8.0/wansuite.egg-info/SOURCES.txt` & `wansuite-9.0/wansuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

