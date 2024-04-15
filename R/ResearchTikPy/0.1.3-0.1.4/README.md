# Comparing `tmp/researchtikpy-0.1.3.tar.gz` & `tmp/researchtikpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "researchtikpy-0.1.3.tar", last modified: Sat Apr 13 16:26:40 2024, max compression
+gzip compressed data, was "researchtikpy-0.1.4.tar", last modified: Mon Apr 15 06:49:08 2024, max compression
```

## Comparing `researchtikpy-0.1.3.tar` & `researchtikpy-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 16:26:40.960799 researchtikpy-0.1.3/
--rw-rw-rw-   0        0        0     1091 2024-04-10 20:07:18.000000 researchtikpy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      413 2024-04-13 16:26:40.958794 researchtikpy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    11190 2024-04-13 15:23:28.000000 researchtikpy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 16:26:40.957794 researchtikpy-0.1.3/ResearchTikPy.egg-info/
--rw-rw-rw-   0        0        0      413 2024-04-13 16:26:40.000000 researchtikpy-0.1.3/ResearchTikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2024-04-13 16:26:40.000000 researchtikpy-0.1.3/ResearchTikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 16:26:40.000000 researchtikpy-0.1.3/ResearchTikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-13 16:26:40.000000 researchtikpy-0.1.3/ResearchTikPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-13 16:26:40.000000 researchtikpy-0.1.3/ResearchTikPy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 16:26:40.955836 researchtikpy-0.1.3/researchtikpy/
--rw-rw-rw-   0        0        0      225 2024-04-13 16:25:19.000000 researchtikpy-0.1.3/researchtikpy/__init__.py
--rw-rw-rw-   0        0        0     4039 2024-04-13 15:00:22.000000 researchtikpy-0.1.3/researchtikpy/get_followers.py
--rw-rw-rw-   0        0        0     2782 2024-04-13 15:01:43.000000 researchtikpy-0.1.3/researchtikpy/get_following.py
--rw-rw-rw-   0        0        0     3211 2024-04-13 15:01:52.000000 researchtikpy-0.1.3/researchtikpy/get_liked_videos.py
--rw-rw-rw-   0        0        0     2279 2024-04-13 15:02:02.000000 researchtikpy-0.1.3/researchtikpy/get_pinned_videos.py
--rw-rw-rw-   0        0        0     1248 2024-04-13 15:02:10.000000 researchtikpy-0.1.3/researchtikpy/get_token.py
--rw-rw-rw-   0        0        0     1889 2024-04-13 15:02:21.000000 researchtikpy-0.1.3/researchtikpy/get_users_info.py
--rw-rw-rw-   0        0        0     2798 2024-04-13 15:02:32.000000 researchtikpy-0.1.3/researchtikpy/get_video_comments.py
--rw-rw-rw-   0        0        0     3576 2024-04-13 15:02:43.000000 researchtikpy-0.1.3/researchtikpy/get_videos_hashtag.py
--rw-rw-rw-   0        0        0     2990 2024-04-13 15:02:53.000000 researchtikpy-0.1.3/researchtikpy/get_videos_info.py
--rw-rw-rw-   0        0        0       42 2024-04-13 16:26:40.960799 researchtikpy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      541 2024-04-13 16:26:17.000000 researchtikpy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:49:08.151650 researchtikpy-0.1.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-10 20:07:18.000000 researchtikpy-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      391 2024-04-15 06:49:08.150517 researchtikpy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11167 2024-04-15 06:31:26.000000 researchtikpy-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 06:49:08.149417 researchtikpy-0.1.4/ResearchTikPy.egg-info/
+-rw-rw-rw-   0        0        0      391 2024-04-15 06:49:07.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-15 06:49:08.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 06:49:07.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 06:49:07.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 06:49:07.000000 researchtikpy-0.1.4/ResearchTikPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 06:49:08.147779 researchtikpy-0.1.4/researchtikpy/
+-rw-rw-rw-   0        0        0      225 2024-04-13 16:25:19.000000 researchtikpy-0.1.4/researchtikpy/__init__.py
+-rw-rw-rw-   0        0        0     1248 2024-04-13 15:02:10.000000 researchtikpy-0.1.4/researchtikpy/get_access_token.py
+-rw-rw-rw-   0        0        0     4039 2024-04-13 15:00:22.000000 researchtikpy-0.1.4/researchtikpy/get_followers.py
+-rw-rw-rw-   0        0        0     2776 2024-04-15 06:01:40.000000 researchtikpy-0.1.4/researchtikpy/get_following.py
+-rw-rw-rw-   0        0        0     3211 2024-04-13 15:01:52.000000 researchtikpy-0.1.4/researchtikpy/get_liked_videos.py
+-rw-rw-rw-   0        0        0     2279 2024-04-13 15:02:02.000000 researchtikpy-0.1.4/researchtikpy/get_pinned_videos.py
+-rw-rw-rw-   0        0        0     1889 2024-04-13 15:02:21.000000 researchtikpy-0.1.4/researchtikpy/get_users_info.py
+-rw-rw-rw-   0        0        0     2798 2024-04-13 15:02:32.000000 researchtikpy-0.1.4/researchtikpy/get_video_comments.py
+-rw-rw-rw-   0        0        0     3570 2024-04-15 06:02:51.000000 researchtikpy-0.1.4/researchtikpy/get_videos_hashtag.py
+-rw-rw-rw-   0        0        0     2990 2024-04-13 15:02:53.000000 researchtikpy-0.1.4/researchtikpy/get_videos_info.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 06:49:08.152192 researchtikpy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-04-15 06:16:22.000000 researchtikpy-0.1.4/setup.py
```

### Comparing `researchtikpy-0.1.3/LICENSE` & `researchtikpy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.3/README.md` & `researchtikpy-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,29 +35,31 @@
    
 
 ## Installation
 
 Currently, ResearchTikPy is not available on PyPI, so it needs to be installed directly from the source:
 
 ```bash
-git clone https://github.com/HohnerJulian/ResearchTikPy.git
-cd ResearchTikPy
-pip install .
+# Install
+pip install ResearchTikPy
+
+# Import
+import ResearchTikPy
 ```
 ## Generating access token
 
 Before using ResearchTikPy, you must obtain access credentials (client key and secret) from TikTok's developer platform. Once you have your credentials, you can use the library to generate an access token that you need to reference every time you run a command in this library:
 
 ```bash
 # It is advised to store your tokens in separate objects or save them in your system's environment to avoid accidental publication of the credentials.
 
 client_key = 'your_client_key'
 client_secet = 'your_client_secret'
 
-access_token = get_access_token(client_krey, client_secret)
+access_token = get_access_token(client_key, client_secret)
 
 # OR paste the credentials within the command
 
 access_token = get_access_token('your_client_key', 'your_client_secret')
 
 
 # print(access_token) # Testing, if necessary. It should look something like this:
```

### Comparing `researchtikpy-0.1.3/ResearchTikPy.egg-info/SOURCES.txt` & `researchtikpy-0.1.4/ResearchTikPy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 setup.py
 ResearchTikPy.egg-info/PKG-INFO
 ResearchTikPy.egg-info/SOURCES.txt
 ResearchTikPy.egg-info/dependency_links.txt
 ResearchTikPy.egg-info/requires.txt
 ResearchTikPy.egg-info/top_level.txt
 researchtikpy/__init__.py
+researchtikpy/get_access_token.py
 researchtikpy/get_followers.py
 researchtikpy/get_following.py
 researchtikpy/get_liked_videos.py
 researchtikpy/get_pinned_videos.py
-researchtikpy/get_token.py
 researchtikpy/get_users_info.py
 researchtikpy/get_video_comments.py
 researchtikpy/get_videos_hashtag.py
 researchtikpy/get_videos_info.py
```

### Comparing `researchtikpy-0.1.3/researchtikpy/get_followers.py` & `researchtikpy-0.1.4/researchtikpy/get_followers.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.3/researchtikpy/get_following.py` & `researchtikpy-0.1.4/researchtikpy/get_following.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # In[5]:
 
 
 import requests
 import pandas as pd
 from time import sleep
 
-def get_following_users(usernames_list, access_token, max_count=100, verbose=True):
+def get_following(usernames_list, access_token, max_count=100, verbose=True):
     """
     Fetches accounts that a user follows. Each username in the list is used to fetch accounts they follow.
 
     Parameters:
     - usernames_list (list): List of usernames to fetch followed accounts for.
     - access_token (str): Access token for TikTok's API.
     - max_count (int): Maximum number of followed accounts to retrieve per request (default 100).
```

### Comparing `researchtikpy-0.1.3/researchtikpy/get_liked_videos.py` & `researchtikpy-0.1.4/researchtikpy/get_liked_videos.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.3/researchtikpy/get_pinned_videos.py` & `researchtikpy-0.1.4/researchtikpy/get_pinned_videos.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.3/researchtikpy/get_token.py` & `researchtikpy-0.1.4/researchtikpy/get_access_token.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.3/researchtikpy/get_users_info.py` & `researchtikpy-0.1.4/researchtikpy/get_users_info.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.3/researchtikpy/get_video_comments.py` & `researchtikpy-0.1.4/researchtikpy/get_video_comments.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.3/researchtikpy/get_videos_hashtag.py` & `researchtikpy-0.1.4/researchtikpy/get_videos_hashtag.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 import requests
 import pandas as pd
 import time
 from datetime import datetime, timedelta
 
-def search_videos_by_hashtag(hashtags, access_token, start_date, end_date, total_max_count, region_code=None, music_id=None, effect_id=None, max_count=100, rate_limit_pause=60):
+def get_videos_hashtag(hashtags, access_token, start_date, end_date, total_max_count, region_code=None, music_id=None, effect_id=None, max_count=100, rate_limit_pause=60):
     """
     Searches for videos by hashtag with optional filters for region code, music ID, or effect ID, and includes rate limit handling. All available fields are retrieved by default, queries are segmented if the range between start_date and end_date exceeds 30 days.
 
     Parameters:
     - hashtags: A list of hashtags to search for.
     - access_token: Your valid access token for the TikTok Research API.
     - start_date: The start date for the search (format YYYYMMDD).
```

### Comparing `researchtikpy-0.1.3/researchtikpy/get_videos_info.py` & `researchtikpy-0.1.4/researchtikpy/get_videos_info.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.3/setup.py` & `researchtikpy-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ResearchTikPy",
-    version="0.1.3",
+    version="0.1.4",
     license="MIT",
     packages=find_packages(),
     install_requires=[
-        "requests", "pandas" 
+        "requests",
+        "pandas"
     ],
     author="Julian Hohner",
     author_email="daswaeldchen@gmail.com",
     description="Python API wrapper for the TikTok Research API",
-    keywords=["TikTok API research", "tiktok", "python3", "api", "tiktok-api", "tiktok api", "tiktok_api", "research"],
-    url="https://github.com/HohnerJulian/ResearchTikPy", 
+    keywords=["TikTok API research", "tiktok", "python3", "api", "tiktok-api", "research"],
+    url="https://github.com/HohnerJulian/ResearchTikPy",
 )
```

