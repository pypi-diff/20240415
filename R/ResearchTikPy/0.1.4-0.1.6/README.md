# Comparing `tmp/researchtikpy-0.1.4.tar.gz` & `tmp/researchtikpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "researchtikpy-0.1.4.tar", last modified: Mon Apr 15 06:49:08 2024, max compression
+gzip compressed data, was "researchtikpy-0.1.6.tar", last modified: Mon Apr 15 13:06:13 2024, max compression
```

## Comparing `researchtikpy-0.1.4.tar` & `researchtikpy-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 06:49:08.151650 researchtikpy-0.1.4/
--rw-rw-rw-   0        0        0     1091 2024-04-10 20:07:18.000000 researchtikpy-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      391 2024-04-15 06:49:08.150517 researchtikpy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    11167 2024-04-15 06:31:26.000000 researchtikpy-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 06:49:08.149417 researchtikpy-0.1.4/ResearchTikPy.egg-info/
--rw-rw-rw-   0        0        0      391 2024-04-15 06:49:07.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-15 06:49:08.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 06:49:07.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 06:49:07.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 06:49:07.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 06:49:08.147779 researchtikpy-0.1.4/researchtikpy/
--rw-rw-rw-   0        0        0      225 2024-04-13 16:25:19.000000 researchtikpy-0.1.4/researchtikpy/__init__.py
--rw-rw-rw-   0        0        0     1248 2024-04-13 15:02:10.000000 researchtikpy-0.1.4/researchtikpy/get_access_token.py
--rw-rw-rw-   0        0        0     4039 2024-04-13 15:00:22.000000 researchtikpy-0.1.4/researchtikpy/get_followers.py
--rw-rw-rw-   0        0        0     2776 2024-04-15 06:01:40.000000 researchtikpy-0.1.4/researchtikpy/get_following.py
--rw-rw-rw-   0        0        0     3211 2024-04-13 15:01:52.000000 researchtikpy-0.1.4/researchtikpy/get_liked_videos.py
--rw-rw-rw-   0        0        0     2279 2024-04-13 15:02:02.000000 researchtikpy-0.1.4/researchtikpy/get_pinned_videos.py
--rw-rw-rw-   0        0        0     1889 2024-04-13 15:02:21.000000 researchtikpy-0.1.4/researchtikpy/get_users_info.py
--rw-rw-rw-   0        0        0     2798 2024-04-13 15:02:32.000000 researchtikpy-0.1.4/researchtikpy/get_video_comments.py
--rw-rw-rw-   0        0        0     3570 2024-04-15 06:02:51.000000 researchtikpy-0.1.4/researchtikpy/get_videos_hashtag.py
--rw-rw-rw-   0        0        0     2990 2024-04-13 15:02:53.000000 researchtikpy-0.1.4/researchtikpy/get_videos_info.py
--rw-rw-rw-   0        0        0       42 2024-04-15 06:49:08.152192 researchtikpy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      520 2024-04-15 06:16:22.000000 researchtikpy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 13:06:13.908471 researchtikpy-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-10 20:07:18.000000 researchtikpy-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0    12115 2024-04-15 13:06:13.906955 researchtikpy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11167 2024-04-15 06:31:26.000000 researchtikpy-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 13:06:13.906444 researchtikpy-0.1.6/ResearchTikPy.egg-info/
+-rw-rw-rw-   0        0        0    12115 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1125 2024-04-15 13:03:19.000000 researchtikpy-0.1.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-15 13:06:13.905405 researchtikpy-0.1.6/researchtikpy/
+-rw-rw-rw-   0        0        0        0 2024-04-15 08:42:07.000000 researchtikpy-0.1.6/researchtikpy/__init__.py
+-rw-rw-rw-   0        0        0     1248 2024-04-13 15:02:10.000000 researchtikpy-0.1.6/researchtikpy/get_access_token.py
+-rw-rw-rw-   0        0        0     4039 2024-04-13 15:00:22.000000 researchtikpy-0.1.6/researchtikpy/get_followers.py
+-rw-rw-rw-   0        0        0     2776 2024-04-15 06:01:40.000000 researchtikpy-0.1.6/researchtikpy/get_following.py
+-rw-rw-rw-   0        0        0     3211 2024-04-13 15:01:52.000000 researchtikpy-0.1.6/researchtikpy/get_liked_videos.py
+-rw-rw-rw-   0        0        0     2279 2024-04-13 15:02:02.000000 researchtikpy-0.1.6/researchtikpy/get_pinned_videos.py
+-rw-rw-rw-   0        0        0     1889 2024-04-13 15:02:21.000000 researchtikpy-0.1.6/researchtikpy/get_users_info.py
+-rw-rw-rw-   0        0        0     2798 2024-04-13 15:02:32.000000 researchtikpy-0.1.6/researchtikpy/get_video_comments.py
+-rw-rw-rw-   0        0        0     3570 2024-04-15 06:02:51.000000 researchtikpy-0.1.6/researchtikpy/get_videos_hashtag.py
+-rw-rw-rw-   0        0        0     2990 2024-04-13 15:02:53.000000 researchtikpy-0.1.6/researchtikpy/get_videos_info.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 13:06:13.908471 researchtikpy-0.1.6/setup.cfg
```

### Comparing `researchtikpy-0.1.4/LICENSE` & `researchtikpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/README.md` & `researchtikpy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/ResearchTikPy.egg-info/SOURCES.txt` & `researchtikpy-0.1.6/ResearchTikPy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
 ResearchTikPy.egg-info/PKG-INFO
 ResearchTikPy.egg-info/SOURCES.txt
 ResearchTikPy.egg-info/dependency_links.txt
 ResearchTikPy.egg-info/requires.txt
 ResearchTikPy.egg-info/top_level.txt
 researchtikpy/__init__.py
 researchtikpy/get_access_token.py
```

### Comparing `researchtikpy-0.1.4/researchtikpy/get_access_token.py` & `researchtikpy-0.1.6/researchtikpy/get_access_token.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/researchtikpy/get_followers.py` & `researchtikpy-0.1.6/researchtikpy/get_followers.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/researchtikpy/get_following.py` & `researchtikpy-0.1.6/researchtikpy/get_following.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/researchtikpy/get_liked_videos.py` & `researchtikpy-0.1.6/researchtikpy/get_liked_videos.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/researchtikpy/get_pinned_videos.py` & `researchtikpy-0.1.6/researchtikpy/get_pinned_videos.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/researchtikpy/get_users_info.py` & `researchtikpy-0.1.6/researchtikpy/get_users_info.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/researchtikpy/get_video_comments.py` & `researchtikpy-0.1.6/researchtikpy/get_video_comments.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/researchtikpy/get_videos_hashtag.py` & `researchtikpy-0.1.6/researchtikpy/get_videos_hashtag.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.4/researchtikpy/get_videos_info.py` & `researchtikpy-0.1.6/researchtikpy/get_videos_info.py`

 * *Files identical despite different names*

