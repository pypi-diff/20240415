# Comparing `tmp/wansuite-7.0.tar.gz` & `tmp/wansuite-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wansuite-7.0.tar", last modified: Mon Apr 15 11:57:56 2024, max compression
+gzip compressed data, was "wansuite-8.0.tar", last modified: Mon Apr 15 13:04:09 2024, max compression
```

## Comparing `wansuite-7.0.tar` & `wansuite-8.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 11:57:56.000000 wansuite-7.0/
--rw-rw-rw-   0        0        0      206 2024-04-15 11:57:56.000000 wansuite-7.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 11:57:56.000000 wansuite-7.0/setup.cfg
--rw-rw-rw-   0        0        0      468 2024-04-15 11:57:52.000000 wansuite-7.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite/
--rw-rw-rw-   0        0        0      102 2024-04-13 14:15:03.000000 wansuite-7.0/wansuite/__init__.py
--rw-rw-rw-   0        0        0    13166 2023-04-03 00:00:42.000000 wansuite-7.0/wansuite/investing.py
--rw-rw-rw-   0        0        0       89 2023-02-10 12:37:51.000000 wansuite-7.0/wansuite/iofile.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite/macrodata/
--rw-rw-rw-   0        0        0       30 2024-04-13 11:06:09.000000 wansuite-7.0/wansuite/macrodata/__init__.py
--rw-rw-rw-   0        0        0     7979 2024-03-15 09:32:37.000000 wansuite-7.0/wansuite/macrodata/updatefromfile.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite/marketdata/
--rw-rw-rw-   0        0        0       30 2024-04-13 11:06:40.000000 wansuite-7.0/wansuite/marketdata/__init__.py
--rw-rw-rw-   0        0        0    10788 2024-04-08 01:56:37.000000 wansuite-7.0/wansuite/marketdata/updateMarketData.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite/media/
--rw-rw-rw-   0        0        0      247 2024-03-31 04:27:38.000000 wansuite-7.0/wansuite/media/__init__.py
--rw-rw-rw-   0        0        0     2259 2024-03-11 04:23:20.000000 wansuite-7.0/wansuite/media/datacollection.py
--rw-rw-rw-   0        0        0      927 2024-03-10 04:22:20.000000 wansuite-7.0/wansuite/media/datavis.py
--rw-rw-rw-   0        0        0        0 2024-03-10 01:20:48.000000 wansuite-7.0/wansuite/media/network.py
--rw-rw-rw-   0        0        0     4625 2024-04-01 00:06:35.000000 wansuite-7.0/wansuite/media/nownews.py
--rw-rw-rw-   0        0        0        0 2024-03-10 01:19:33.000000 wansuite-7.0/wansuite/media/sentiment.py
--rw-rw-rw-   0        0        0      284 2024-03-09 23:27:15.000000 wansuite-7.0/wansuite/media/sys.py
--rw-rw-rw-   0        0        0     2508 2024-03-10 23:57:19.000000 wansuite-7.0/wansuite/media/textfeature.py
--rw-rw-rw-   0        0        0     2765 2024-03-10 23:27:24.000000 wansuite-7.0/wansuite/media/textprocessing.py
--rw-rw-rw-   0        0        0      512 2024-03-10 01:50:26.000000 wansuite-7.0/wansuite/media/topicmodel.py
--rw-rw-rw-   0        0        0     3659 2024-03-07 16:43:29.000000 wansuite-7.0/wansuite/msql.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite/order/
--rw-rw-rw-   0        0        0        0 2024-03-08 01:36:18.000000 wansuite-7.0/wansuite/order/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite/strategy/
--rw-rw-rw-   0        0        0       18 2024-04-13 11:07:03.000000 wansuite-7.0/wansuite/strategy/__init__.py
--rw-rw-rw-   0        0        0    21210 2024-03-25 13:03:06.000000 wansuite-7.0/wansuite/strategy/zack.py
--rw-rw-rw-   0        0        0      122 2024-04-15 11:23:57.000000 wansuite-7.0/wansuite/sys.py
--rw-rw-rw-   0        0        0      397 2023-02-08 13:29:16.000000 wansuite-7.0/wansuite/wtime.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite.egg-info/
--rw-rw-rw-   0        0        0      206 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      783 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 11:57:56.000000 wansuite-7.0/wansuite.egg-info/top_level.txt
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.179399 wansuite-8.0/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       83 2024-04-15 13:04:09.179263 wansuite-8.0/PKG-INFO
+-rw-r--r--   0 neuronpro   (501) staff       (20)       38 2024-04-15 13:04:09.179442 wansuite-8.0/setup.cfg
+-rw-r--r--   0 neuronpro   (501) staff       (20)      468 2024-04-15 13:04:06.000000 wansuite-8.0/setup.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.176180 wansuite-8.0/wansuite/
+-rw-r--r--   0 neuronpro   (501) staff       (20)      102 2024-04-13 14:15:03.000000 wansuite-8.0/wansuite/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)    13166 2023-04-03 00:00:42.000000 wansuite-8.0/wansuite/investing.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)       89 2023-02-10 12:37:51.000000 wansuite-8.0/wansuite/iofile.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.177120 wansuite-8.0/wansuite/macrodata/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       30 2024-04-13 11:06:09.000000 wansuite-8.0/wansuite/macrodata/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     7979 2024-03-15 09:32:37.000000 wansuite-8.0/wansuite/macrodata/updatefromfile.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.177448 wansuite-8.0/wansuite/marketdata/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       30 2024-04-13 11:06:40.000000 wansuite-8.0/wansuite/marketdata/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)    10788 2024-04-08 01:56:37.000000 wansuite-8.0/wansuite/marketdata/updateMarketData.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.178719 wansuite-8.0/wansuite/media/
+-rw-r--r--   0 neuronpro   (501) staff       (20)      247 2024-03-31 04:27:38.000000 wansuite-8.0/wansuite/media/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     2259 2024-03-11 04:23:20.000000 wansuite-8.0/wansuite/media/datacollection.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      927 2024-03-10 04:22:20.000000 wansuite-8.0/wansuite/media/datavis.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)        0 2024-03-10 01:20:48.000000 wansuite-8.0/wansuite/media/network.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     4625 2024-04-01 00:06:35.000000 wansuite-8.0/wansuite/media/nownews.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)        0 2024-03-10 01:19:33.000000 wansuite-8.0/wansuite/media/sentiment.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      284 2024-03-09 23:27:15.000000 wansuite-8.0/wansuite/media/sys.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     2508 2024-03-10 23:57:19.000000 wansuite-8.0/wansuite/media/textfeature.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     2765 2024-03-10 23:27:24.000000 wansuite-8.0/wansuite/media/textprocessing.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      512 2024-03-10 01:50:26.000000 wansuite-8.0/wansuite/media/topicmodel.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)     3659 2024-03-07 16:43:29.000000 wansuite-8.0/wansuite/msql.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.178844 wansuite-8.0/wansuite/order/
+-rw-r--r--   0 neuronpro   (501) staff       (20)        0 2024-03-08 01:36:18.000000 wansuite-8.0/wansuite/order/__init__.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.179061 wansuite-8.0/wansuite/strategy/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       18 2024-04-13 11:07:03.000000 wansuite-8.0/wansuite/strategy/__init__.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)    21210 2024-03-25 13:03:06.000000 wansuite-8.0/wansuite/strategy/zack.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      122 2024-04-15 11:23:57.000000 wansuite-8.0/wansuite/sys.py
+-rw-r--r--   0 neuronpro   (501) staff       (20)      397 2023-02-08 13:29:16.000000 wansuite-8.0/wansuite/wtime.py
+drwxr-xr-x   0 neuronpro   (501) staff       (20)        0 2024-04-15 13:04:09.176857 wansuite-8.0/wansuite.egg-info/
+-rw-r--r--   0 neuronpro   (501) staff       (20)       83 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/PKG-INFO
+-rw-r--r--   0 neuronpro   (501) staff       (20)      783 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/SOURCES.txt
+-rw-r--r--   0 neuronpro   (501) staff       (20)        1 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/dependency_links.txt
+-rw-r--r--   0 neuronpro   (501) staff       (20)      111 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/requires.txt
+-rw-r--r--   0 neuronpro   (501) staff       (20)        9 2024-04-15 13:04:09.000000 wansuite-8.0/wansuite.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wansuite-7.0/wansuite/investing.py` & `wansuite-8.0/wansuite/investing.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/macrodata/updatefromfile.py` & `wansuite-8.0/wansuite/macrodata/updatefromfile.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/marketdata/updateMarketData.py` & `wansuite-8.0/wansuite/marketdata/updateMarketData.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/media/datacollection.py` & `wansuite-8.0/wansuite/media/datacollection.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/media/datavis.py` & `wansuite-8.0/wansuite/media/datavis.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/media/nownews.py` & `wansuite-8.0/wansuite/media/nownews.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/media/textfeature.py` & `wansuite-8.0/wansuite/media/textfeature.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/media/textprocessing.py` & `wansuite-8.0/wansuite/media/textprocessing.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/media/topicmodel.py` & `wansuite-8.0/wansuite/media/topicmodel.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/msql.py` & `wansuite-8.0/wansuite/msql.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite/strategy/zack.py` & `wansuite-8.0/wansuite/strategy/zack.py`

 * *Files identical despite different names*

### Comparing `wansuite-7.0/wansuite.egg-info/SOURCES.txt` & `wansuite-8.0/wansuite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

