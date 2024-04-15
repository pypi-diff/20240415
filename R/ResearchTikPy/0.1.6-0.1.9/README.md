# Comparing `tmp/researchtikpy-0.1.6.tar.gz` & `tmp/researchtikpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "researchtikpy-0.1.6.tar", last modified: Mon Apr 15 13:06:13 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `researchtikpy-0.1.6.tar` & `researchtikpy-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 13:06:13.908471 researchtikpy-0.1.6/
--rw-rw-rw-   0        0        0     1091 2024-04-10 20:07:18.000000 researchtikpy-0.1.6/LICENSE
--rw-rw-rw-   0        0        0    12115 2024-04-15 13:06:13.906955 researchtikpy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    11167 2024-04-15 06:31:26.000000 researchtikpy-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 13:06:13.906444 researchtikpy-0.1.6/ResearchTikPy.egg-info/
--rw-rw-rw-   0        0        0    12115 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-15 13:06:13.000000 researchtikpy-0.1.6/ResearchTikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1125 2024-04-15 13:03:19.000000 researchtikpy-0.1.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-15 13:06:13.905405 researchtikpy-0.1.6/researchtikpy/
--rw-rw-rw-   0        0        0        0 2024-04-15 08:42:07.000000 researchtikpy-0.1.6/researchtikpy/__init__.py
--rw-rw-rw-   0        0        0     1248 2024-04-13 15:02:10.000000 researchtikpy-0.1.6/researchtikpy/get_access_token.py
--rw-rw-rw-   0        0        0     4039 2024-04-13 15:00:22.000000 researchtikpy-0.1.6/researchtikpy/get_followers.py
--rw-rw-rw-   0        0        0     2776 2024-04-15 06:01:40.000000 researchtikpy-0.1.6/researchtikpy/get_following.py
--rw-rw-rw-   0        0        0     3211 2024-04-13 15:01:52.000000 researchtikpy-0.1.6/researchtikpy/get_liked_videos.py
--rw-rw-rw-   0        0        0     2279 2024-04-13 15:02:02.000000 researchtikpy-0.1.6/researchtikpy/get_pinned_videos.py
--rw-rw-rw-   0        0        0     1889 2024-04-13 15:02:21.000000 researchtikpy-0.1.6/researchtikpy/get_users_info.py
--rw-rw-rw-   0        0        0     2798 2024-04-13 15:02:32.000000 researchtikpy-0.1.6/researchtikpy/get_video_comments.py
--rw-rw-rw-   0        0        0     3570 2024-04-15 06:02:51.000000 researchtikpy-0.1.6/researchtikpy/get_videos_hashtag.py
--rw-rw-rw-   0        0        0     2990 2024-04-13 15:02:53.000000 researchtikpy-0.1.6/researchtikpy/get_videos_info.py
--rw-rw-rw-   0        0        0       42 2024-04-15 13:06:13.908471 researchtikpy-0.1.6/setup.cfg
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/requirements.txt
+-rw-r--r--   0        0        0    51875 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/images/Package_logo.png
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/__init__.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/get_access_token.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/get_followers.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/get_following.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/get_liked_videos.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/get_pinned_videos.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/get_users_info.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/get_video_comments.py
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/get_videos_hashtag.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/src/researchtikpy/get_videos_info.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/LICENSE
+-rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/README.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 researchtikpy-0.1.9/PKG-INFO
```

### Comparing `researchtikpy-0.1.6/LICENSE` & `researchtikpy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/PKG-INFO` & `researchtikpy-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,283 +1,275 @@
-Metadata-Version: 2.1
-Name: ResearchTikPy
-Version: 0.1.6
-Summary: Python API wrapper for the TikTok Research API
-Author-email: Hohner Julian <daswaeldchen@gmail.com>
-Project-URL: homepage, https://github.com/HohnerJulian/ResearchTikPy
-Keywords: TikTok API research,tiktok,python3,api,tiktok-api,research
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.26.0
-Requires-Dist: pandas
-
-
-![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)
-![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)
-![PyPI Version](https://img.shields.io/pypi/v/ResearchTikPy.svg)
-![License](https://img.shields.io/badge/license-MIT-green.svg)
-![LinkedIn Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/julian-hohner-71a93b163/)
-[![X](https://img.shields.io/badge/X-%23000000.svg?style=for-the-badge&logo=X&logoColor=white)](https://twitter.com/J_H_ohner)
-
-
-<p align="middle">
-  <img src="/images/Package_logo.png" width="400" /> <!-- Adjust width as needed -->
-</p>
-
-ResearchTikPy is a Python library designed to facilitate access to [TikTok's Research API](https://developers.tiktok.com/products/research-api/), providing a simple and intuitive interface for collecting data on videos, users, comments, and more. This library is intended for academic and research purposes, aiming to streamline the data collection process from TikTok without directly interfering with the API.
-
-**Features of ResearchTikPy:**
-
-| Includes                                        | Does Not (Yet) Include                                 |
-|-------------------------------------------------|--------------------------------------------------------|
-| [Fetch video infos by key term(s)](#keyterm_search) | Downloading videos                                 |       
-| [Fetching user information](#get_users_info) | Extracting text from videos (OCR)                         |
-| [Search for videos by user(s)](#get_videos_info) | Downloading sounds of videos                          |
-| [Collecting comments from videos](#get_video_comments) |                                                 |
-| [Fetching the followers of accounts](#get_followers)  |                                                  |
-| [Fetching accounts followed by a user](#get_following_users) |                                           |
-| [Fetching videos liked by a user](#get_liked_videos) |                                                   |
-| [Fetching videos pinned by a user](#get_pinned_videos) |                                                 |
-<br><br>
-
-### Word of Caution 
-
-1. Splitting your requests into smaller chunks is generally advised to avoid longer fetching times and data loss.
-2. Read [TikTok's guide](https://developers.tiktok.com/doc/about-research-api/) about the research API to inform you about restrictions, daily quotas and FAQs.
-3. Feel free to contact me or submit a question in case you encounter bugs or errors!
-   
-
-## Installation
-
-Currently, ResearchTikPy is not available on PyPI, so it needs to be installed directly from the source:
-
-```bash
-# Install
-pip install ResearchTikPy
-
-# Import
-import ResearchTikPy
-```
-## Generating access token
-
-Before using ResearchTikPy, you must obtain access credentials (client key and secret) from TikTok's developer platform. Once you have your credentials, you can use the library to generate an access token that you need to reference every time you run a command in this library:
-
-```bash
-# It is advised to store your tokens in separate objects or save them in your system's environment to avoid accidental publication of the credentials.
-
-client_key = 'your_client_key'
-client_secet = 'your_client_secret'
-
-access_token = get_access_token(client_key, client_secret)
-
-# OR paste the credentials within the command
-
-access_token = get_access_token('your_client_key', 'your_client_secret')
-
-
-# print(access_token) # Testing, if necessary. It should look something like this:
-
-
-#Access Token: clt.Vl7HEasdfdeX28Z0G4wervRoPpY5f3zAGgYmGAAyGkowkYCusgbwqmb4NtNzn2QstXh
-#Expires In: 7200
-#Token Type: Bearer
-
-```
-
-# Features
-This package features every possible query currently provided by the Researcher API of TikTok. For the full documentation, including a list of variables, see the official [Codebook](https://developers.tiktok.com/doc/research-api-codebook)
-
-
-<br><br>
-
-<a name="keyterm_search"></a>
-### Function: **Keyterm search**
-
-Fetches video information by hashtag. 
-
-```bash
-videos_df = search_videos_by_hashtag(hashtags, access_token, start_date, end_date, total_max_videos (optional),
-     region_code (optional), music_id (optional), effect_id (optional), max_count (optional),  rate_limit_pause (optional))
-```
-
-Parameters: 
-
-* **hashtags**: A list of hashtag(s) to search for, e.g., "FYP" or ["FYP", "FORYOURPAGE"].
-* **access_token**: Your valid access token for the TikTok Research API. Stored as a string.
-* **start_date**: The start date for the search. The format should be 'YYYYMMDD'.
-* **end_date**: The end date for the search. The format should be 'YYYYMMDD'.
-* **total_max_count** (Optional): The total maximum number of videos to collect. **Keeping this within a manageable range is advised because of the fetching duration and daily quota limit! The default is infinite.** Stored as an integer, e.g., 500.
-* **region_code** (Optional): The region code to filter videos by. See list of [region_codes](https://developers.tiktok.com/doc/research-api-specs-query-videos).
-* **music_id** (Optional): The music ID to filter videos by. Stored as a string.
-* **effect_id** (Optional): The effect ID to filter videos by. Stored as a string.
-* **max_count** (Optional):  The maximum number of videos to return **per individual get request** (default & max is 100). 
-* **rate_limit_pause** (Optional):  Time in seconds to wait when a rate limit error is encountered. The default is 60 seconds. It can be adjusted as you like, e.g., 30.
-
-<br><br>
-
-<a name="get_users_info"></a>
-### Function: **get_users_info**
-
-Collect user information. Possible parameters are: 
-
-```bash
-user_df = get_users_info(usernames, access_token, start_date, end_date)
-```
-
-Fetches account information for given usernames within the specified date range and compiles them into a single DataFrame.
-
-Parameters:
-
-* **usernames**: List of username(s) to fetch videos for.
-* **access_token**: Authorization token for TikTok Research API.
-* **max_count** (Optional): Maximum number of videos to return per request (default is 100).
-* **verbose** (Optional): If True (default), prints detailed logs; if False, suppresses most print statements.
-
-<br><br>
-
-<a name="get_videos_info"></a>
-### Function: **get_videos_info**
-
-Fetches all videos & video metadata of an account or accounts and compiles them into a single DataFrame (with account IDs).
-
-```bash
-videos_df = get_videos_info(usernames, access_token, fields (optional), start_date(optional), end_date(optional), max_count(optional))
-```
-
-Parameters:
-- **usernames**: List of usernames to fetch videos for.
-- **access_token**: Authorization token for TikTok Research API.
-- **start_date**: The start date for the video search (format YYYYMMDD).
-- **end_date**: End date for the video search (format YYYYMMDD).
-- **max_count** (Optional): Maximum number of videos to return per request (default is 100).
-- **verbose** (Optional): If True (default), prints detailed logs; if False, suppresses most print statements.
-
-<br><br>
-
-<a name="get_video_comments"></a>
-### Function: **get_video_comments**
-
-Fetches comments on video(s) and compiles them into a single DataFrame (with video IDs).
-
-```bash
-comments_df = get_video_comments(videos_df, access_token, fields (optional), max_count (optional), verbose (optional))
-```
-Parameters:
-* **videos_df**: DataFrame with a column 'id' containing video IDs (f.e. provided by `get_videos_info`).
-* **access_token**: Authorization token for TikTok Research API.
-* **fields** (optional)
-* **max_count** (optional)
-* **verbose** (optional)
-
-<br><br>
-
-<a name="get_pinned_videos"></a>
-### Function: **get_pinned_videos**
-
-Fetches pinned videos of accounts and compiles them into a single DataFrame.
-
-```bash
-pinned_df = get_pinned_videos(usernames, access_token, fields (optional), max_count (optional), verbose (optional))
-```
-
-* **usernames**: List of usernames to fetch videos for. Reports no pinned videos if account has none. 
-* **access_token**: Authorization token for TikTok Research API.
-* **fields** (optional)
-* **verbose** (optional)
-
-<br><br>
-
-<a name="get_liked_videos"></a>
-### Function: **get_liked_videos**
-
-Fetches metadata of videos accounts have like. Only works if accounts enabled this feature. If an account has not enabled this, the section on his profil pages is keyed out and a lock symbol is placed there. 
-
-```bash
-liked_df = get_liked_videos(usernames, access_token, fields (optional), max_count (optional), verbose (optional))
-```
-Parameters:
-* **usernames**: List of usernames to fetch videos for. Reports no liked videos if account has none. 
-* **access_token**: Authorization token for TikTok Research API.
-* **fields** (optional)
-* **max_count** (optional)
-* **verbose** (optional)
-
-<br><br>
-
-<a name="get_following_users"></a>
-### Function: **get_following_users**
-
-Fetches followers of accounts and compiles them into a single DataFrame. It is advised to keep the list of usernames short to avoid longer runtimes and to account for the large amount of possible followers!. 
-Compiles them into a single DataFrame with the variable `target_account` indicating the seed account.
-
-```bash
-following = get_following_users (usernames, access_token, fields (optional), max_count (optional), verbose (optional))
-```
-Parameters:
-* **usernames**: List of usernames to fetch videos for. Reports no pinned videos if account has none. 
-* **access_token**: Authorization token for TikTok Research API.
-* **fields** (optional)
-* **max_count** (optional)
-* **verbose** (optional)
-
-<br><br>
-
-<a name="get_followers"></a>
-### Function: **get_followers**
-
-Fetches followers for multiple users and compiles them into a single DataFrame. It is advised to keep the list of 
-usernames short to avoid longer runtimes OR to use the `total_count` parameter to avoid reaching daily quotas rather quickly.
-
-```bash
-followers = get_followers (usernames, access_token, total_count (optional) fields (optional), max_count (optional), verbose (optional))
-```
-
-Parameters:
-* **usernames**: List of usernames to fetch videos for. Reports no pinned videos if account has none. 
-* **access_token**: Authorization token for TikTok Research API.
-* **total_count** (optional): Maximum total number of followers to retrieve per user (integer input). 
-* **fields** (optional)
-* **max_count** (optional)
-* **verbose** (optional)
-
-## Cite
-
-Please feel free to cite me when using the package: 
-
-Hohner, J. (2024). ResearchPikTy (Python Library). Github Repository: https://github.com/HohnerJulian/ResearchTikPy
-
-or Bibtex: 
-
-@misc{Hohner2024ResearchTikPy,
-  author = {Hohner, Julian},
-  title = {{ResearchTikPy: Python Library for TikTok's Research API}},
-  year = {2024},
-  howpublished = {\url{https://github.com/HohnerJulian/ResearchTikPy}},
-  note = {Accessed: yyyy-mm-dd}
-}
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+Metadata-Version: 2.3
+Name: ResearchTikPy
+Version: 0.1.9
+Summary: Python API wrapper for the TikTok Research API
+Project-URL: Homepage, https://github.com/HohnerJulian/ResearchTikPy
+Author-email: Julian Hohner <daswaeldchen@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Requires-Dist: pandas
+Requires-Dist: requests
+Description-Content-Type: text/markdown
+
+
+![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)
+![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)
+![PyPI Version](https://img.shields.io/pypi/v/ResearchTikPy.svg)
+![License](https://img.shields.io/badge/license-MIT-green.svg)
+![LinkedIn Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/julian-hohner-71a93b163/)
+[![X](https://img.shields.io/badge/X-%23000000.svg?style=for-the-badge&logo=X&logoColor=white)](https://twitter.com/J_H_ohner)
+
+
+<p align="middle">
+  <img src="/images/Package_logo.png" width="400" /> <!-- Adjust width as needed -->
+</p>
+
+ResearchTikPy is a Python library designed to facilitate access to [TikTok's Research API](https://developers.tiktok.com/products/research-api/), providing a simple and intuitive interface for collecting data on videos, users, comments, and more. This library is intended for academic and research purposes, aiming to streamline the data collection process from TikTok without directly interfering with the API.
+
+**Features of ResearchTikPy:**
+
+| Includes                                        | Does Not (Yet) Include                                 |
+|-------------------------------------------------|--------------------------------------------------------|
+| [Fetch video infos by key term(s)](#keyterm_search) | Downloading videos                                 |       
+| [Fetching user information](#get_users_info) | Extracting text from videos (OCR)                         |
+| [Search for videos by user(s)](#get_videos_info) | Downloading sounds of videos                          |
+| [Collecting comments from videos](#get_video_comments) |                                                 |
+| [Fetching the followers of accounts](#get_followers)  |                                                  |
+| [Fetching accounts followed by a user](#get_following_users) |                                           |
+| [Fetching videos liked by a user](#get_liked_videos) |                                                   |
+| [Fetching videos pinned by a user](#get_pinned_videos) |                                                 |
+<br><br>
+
+### Word of Caution 
+
+1. Splitting your requests into smaller chunks is generally advised to avoid longer fetching times and data loss.
+2. Read [TikTok's guide](https://developers.tiktok.com/doc/about-research-api/) about the research API to inform you about restrictions, daily quotas and FAQs.
+3. Feel free to contact me or submit a question in case you encounter bugs or errors!
+   
+
+## Installation
+
+Currently, ResearchTikPy is not available on PyPI, so it needs to be installed directly from the source:
+
+```bash
+# Install
+pip install ResearchTikPy
+
+# Import
+import ResearchTikPy
+```
+## Generating access token
+
+Before using ResearchTikPy, you must obtain access credentials (client key and secret) from TikTok's developer platform. Once you have your credentials, you can use the library to generate an access token that you need to reference every time you run a command in this library:
+
+```bash
+# It is advised to store your tokens in separate objects or save them in your system's environment to avoid accidental publication of the credentials.
+
+client_key = 'your_client_key'
+client_secet = 'your_client_secret'
+
+access_token = get_access_token(client_key, client_secret)
+
+# OR paste the credentials within the command
+
+access_token = get_access_token('your_client_key', 'your_client_secret')
+
+
+# print(access_token) # Testing, if necessary. It should look something like this:
+
+
+#Access Token: clt.Vl7HEasdfdeX28Z0G4wervRoPpY5f3zAGgYmGAAyGkowkYCusgbwqmb4NtNzn2QstXh
+#Expires In: 7200
+#Token Type: Bearer
+
+```
+
+# Features
+This package features every possible query currently provided by the Researcher API of TikTok. For the full documentation, including a list of variables, see the official [Codebook](https://developers.tiktok.com/doc/research-api-codebook)
+
+
+<br><br>
+
+<a name="keyterm_search"></a>
+### Function: **Keyterm search**
+
+Fetches video information by hashtag. 
+
+```bash
+videos_df = search_videos_by_hashtag(hashtags, access_token, start_date, end_date, total_max_videos (optional),
+     region_code (optional), music_id (optional), effect_id (optional), max_count (optional),  rate_limit_pause (optional))
+```
+
+Parameters: 
+
+* **hashtags**: A list of hashtag(s) to search for, e.g., "FYP" or ["FYP", "FORYOURPAGE"].
+* **access_token**: Your valid access token for the TikTok Research API. Stored as a string.
+* **start_date**: The start date for the search. The format should be 'YYYYMMDD'.
+* **end_date**: The end date for the search. The format should be 'YYYYMMDD'.
+* **total_max_count** (Optional): The total maximum number of videos to collect. **Keeping this within a manageable range is advised because of the fetching duration and daily quota limit! The default is infinite.** Stored as an integer, e.g., 500.
+* **region_code** (Optional): The region code to filter videos by. See list of [region_codes](https://developers.tiktok.com/doc/research-api-specs-query-videos).
+* **music_id** (Optional): The music ID to filter videos by. Stored as a string.
+* **effect_id** (Optional): The effect ID to filter videos by. Stored as a string.
+* **max_count** (Optional):  The maximum number of videos to return **per individual get request** (default & max is 100). 
+* **rate_limit_pause** (Optional):  Time in seconds to wait when a rate limit error is encountered. The default is 60 seconds. It can be adjusted as you like, e.g., 30.
+
+<br><br>
+
+<a name="get_users_info"></a>
+### Function: **get_users_info**
+
+Collect user information. Possible parameters are: 
+
+```bash
+user_df = get_users_info(usernames, access_token, start_date, end_date)
+```
+
+Fetches account information for given usernames within the specified date range and compiles them into a single DataFrame.
+
+Parameters:
+
+* **usernames**: List of username(s) to fetch videos for.
+* **access_token**: Authorization token for TikTok Research API.
+* **max_count** (Optional): Maximum number of videos to return per request (default is 100).
+* **verbose** (Optional): If True (default), prints detailed logs; if False, suppresses most print statements.
+
+<br><br>
+
+<a name="get_videos_info"></a>
+### Function: **get_videos_info**
+
+Fetches all videos & video metadata of an account or accounts and compiles them into a single DataFrame (with account IDs).
+
+```bash
+videos_df = get_videos_info(usernames, access_token, fields (optional), start_date(optional), end_date(optional), max_count(optional))
+```
+
+Parameters:
+- **usernames**: List of usernames to fetch videos for.
+- **access_token**: Authorization token for TikTok Research API.
+- **start_date**: The start date for the video search (format YYYYMMDD).
+- **end_date**: End date for the video search (format YYYYMMDD).
+- **max_count** (Optional): Maximum number of videos to return per request (default is 100).
+- **verbose** (Optional): If True (default), prints detailed logs; if False, suppresses most print statements.
+
+<br><br>
+
+<a name="get_video_comments"></a>
+### Function: **get_video_comments**
+
+Fetches comments on video(s) and compiles them into a single DataFrame (with video IDs).
+
+```bash
+comments_df = get_video_comments(videos_df, access_token, fields (optional), max_count (optional), verbose (optional))
+```
+Parameters:
+* **videos_df**: DataFrame with a column 'id' containing video IDs (f.e. provided by `get_videos_info`).
+* **access_token**: Authorization token for TikTok Research API.
+* **fields** (optional)
+* **max_count** (optional)
+* **verbose** (optional)
+
+<br><br>
+
+<a name="get_pinned_videos"></a>
+### Function: **get_pinned_videos**
+
+Fetches pinned videos of accounts and compiles them into a single DataFrame.
+
+```bash
+pinned_df = get_pinned_videos(usernames, access_token, fields (optional), max_count (optional), verbose (optional))
+```
+
+* **usernames**: List of usernames to fetch videos for. Reports no pinned videos if account has none. 
+* **access_token**: Authorization token for TikTok Research API.
+* **fields** (optional)
+* **verbose** (optional)
+
+<br><br>
+
+<a name="get_liked_videos"></a>
+### Function: **get_liked_videos**
+
+Fetches metadata of videos accounts have like. Only works if accounts enabled this feature. If an account has not enabled this, the section on his profil pages is keyed out and a lock symbol is placed there. 
+
+```bash
+liked_df = get_liked_videos(usernames, access_token, fields (optional), max_count (optional), verbose (optional))
+```
+Parameters:
+* **usernames**: List of usernames to fetch videos for. Reports no liked videos if account has none. 
+* **access_token**: Authorization token for TikTok Research API.
+* **fields** (optional)
+* **max_count** (optional)
+* **verbose** (optional)
+
+<br><br>
+
+<a name="get_following_users"></a>
+### Function: **get_following_users**
+
+Fetches followers of accounts and compiles them into a single DataFrame. It is advised to keep the list of usernames short to avoid longer runtimes and to account for the large amount of possible followers!. 
+Compiles them into a single DataFrame with the variable `target_account` indicating the seed account.
+
+```bash
+following = get_following_users (usernames, access_token, fields (optional), max_count (optional), verbose (optional))
+```
+Parameters:
+* **usernames**: List of usernames to fetch videos for. Reports no pinned videos if account has none. 
+* **access_token**: Authorization token for TikTok Research API.
+* **fields** (optional)
+* **max_count** (optional)
+* **verbose** (optional)
+
+<br><br>
+
+<a name="get_followers"></a>
+### Function: **get_followers**
+
+Fetches followers for multiple users and compiles them into a single DataFrame. It is advised to keep the list of 
+usernames short to avoid longer runtimes OR to use the `total_count` parameter to avoid reaching daily quotas rather quickly.
+
+```bash
+followers = get_followers (usernames, access_token, total_count (optional) fields (optional), max_count (optional), verbose (optional))
+```
+
+Parameters:
+* **usernames**: List of usernames to fetch videos for. Reports no pinned videos if account has none. 
+* **access_token**: Authorization token for TikTok Research API.
+* **total_count** (optional): Maximum total number of followers to retrieve per user (integer input). 
+* **fields** (optional)
+* **max_count** (optional)
+* **verbose** (optional)
+
+## Cite
+
+Please feel free to cite me when using the package: 
+
+Hohner, J. (2024). ResearchPikTy (Python Library). Github Repository: https://github.com/HohnerJulian/ResearchTikPy
+
+or Bibtex: 
+
+@misc{Hohner2024ResearchTikPy,
+  author = {Hohner, Julian},
+  title = {{ResearchTikPy: Python Library for TikTok's Research API}},
+  year = {2024},
+  howpublished = {\url{https://github.com/HohnerJulian/ResearchTikPy}},
+  note = {Accessed: yyyy-mm-dd}
+}
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `researchtikpy-0.1.6/README.md` & `researchtikpy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/researchtikpy/get_access_token.py` & `researchtikpy-0.1.9/src/researchtikpy/get_access_token.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/researchtikpy/get_followers.py` & `researchtikpy-0.1.9/src/researchtikpy/get_followers.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/researchtikpy/get_following.py` & `researchtikpy-0.1.9/src/researchtikpy/get_following.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/researchtikpy/get_liked_videos.py` & `researchtikpy-0.1.9/src/researchtikpy/get_liked_videos.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/researchtikpy/get_pinned_videos.py` & `researchtikpy-0.1.9/src/researchtikpy/get_pinned_videos.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/researchtikpy/get_users_info.py` & `researchtikpy-0.1.9/src/researchtikpy/get_users_info.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/researchtikpy/get_video_comments.py` & `researchtikpy-0.1.9/src/researchtikpy/get_video_comments.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/researchtikpy/get_videos_hashtag.py` & `researchtikpy-0.1.9/src/researchtikpy/get_videos_hashtag.py`

 * *Files identical despite different names*

### Comparing `researchtikpy-0.1.6/researchtikpy/get_videos_info.py` & `researchtikpy-0.1.9/src/researchtikpy/get_videos_info.py`

 * *Files identical despite different names*

