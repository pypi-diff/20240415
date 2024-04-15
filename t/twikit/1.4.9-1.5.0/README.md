# Comparing `tmp/twikit-1.4.9.tar.gz` & `tmp/twikit-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.4.9.tar", last modified: Sun Apr 14 04:30:39 2024, max compression
+gzip compressed data, was "twikit-1.5.0.tar", last modified: Mon Apr 15 14:52:51 2024, max compression
```

## Comparing `twikit-1.4.9.tar` & `twikit-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 04:30:39.649922 twikit-1.4.9/
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.4.9/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-14 04:30:39.647903 twikit-1.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.4.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 04:30:39.649922 twikit-1.4.9/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:30:39.579086 twikit-1.4.9/twikit/
--rw-rw-rw-   0        0        0      509 2024-04-14 04:28:42.000000 twikit-1.4.9/twikit/__init__.py
--rw-rw-rw-   0        0        0   113090 2024-04-14 04:26:41.000000 twikit-1.4.9/twikit/client.py
--rw-rw-rw-   0        0        0     2380 2024-04-13 12:42:36.000000 twikit-1.4.9/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.4.9/twikit/group.py
--rw-rw-rw-   0        0        0     1913 2024-04-13 14:12:05.000000 twikit-1.4.9/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.4.9/twikit/notification.py
--rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/trend.py
--rw-rw-rw-   0        0        0    20706 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:30:39.643915 twikit-1.4.9/twikit/twikit_async/
--rw-rw-rw-   0        0        0      461 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   115055 2024-04-14 04:28:02.000000 twikit-1.4.9/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     1955 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    20105 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-04-14 04:11:42.000000 twikit-1.4.9/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-04-14 04:11:03.000000 twikit-1.4.9/twikit/user.py
--rw-rw-rw-   0        0        0    21797 2024-04-13 12:42:37.000000 twikit-1.4.9/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-14 04:30:39.596040 twikit-1.4.9/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-14 04:30:39.000000 twikit-1.4.9/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-04-14 04:30:39.000000 twikit-1.4.9/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 04:30:39.000000 twikit-1.4.9/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-14 04:30:39.000000 twikit-1.4.9/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-14 04:30:39.000000 twikit-1.4.9/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:51.348049 twikit-1.5.0/
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-15 14:52:51.345054 twikit-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:52:51.349044 twikit-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:51.263274 twikit-1.5.0/twikit/
+-rw-rw-rw-   0        0        0      620 2024-04-15 14:49:26.000000 twikit-1.5.0/twikit/__init__.py
+-rw-rw-rw-   0        0        0   131589 2024-04-15 14:28:49.000000 twikit-1.5.0/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.0/twikit/community.py
+-rw-rw-rw-   0        0        0     2626 2024-04-14 11:15:08.000000 twikit-1.5.0/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.0/twikit/group.py
+-rw-rw-rw-   0        0        0     2095 2024-04-14 11:11:34.000000 twikit-1.5.0/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.0/twikit/notification.py
+-rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/trend.py
+-rw-rw-rw-   0        0        0    20744 2024-04-14 15:05:06.000000 twikit-1.5.0/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:51.342062 twikit-1.5.0/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      572 2024-04-15 14:48:54.000000 twikit-1.5.0/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   133874 2024-04-15 14:40:16.000000 twikit-1.5.0/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.0/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.0/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    20613 2024-04-14 11:18:02.000000 twikit-1.5.0/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-04-14 04:11:42.000000 twikit-1.5.0/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.0/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-04-14 04:11:03.000000 twikit-1.5.0/twikit/user.py
+-rw-rw-rw-   0        0        0    24789 2024-04-15 12:37:05.000000 twikit-1.5.0/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:52:51.287209 twikit-1.5.0/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-15 14:52:50.000000 twikit-1.5.0/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2024-04-15 14:52:51.000000 twikit-1.5.0/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:52:50.000000 twikit-1.5.0/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-15 14:52:50.000000 twikit-1.5.0/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 14:52:50.000000 twikit-1.5.0/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.4.9/LICENSE` & `twikit-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/PKG-INFO` & `twikit-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.9
+Version: 1.5.0
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.9/README.md` & `twikit-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/setup.py` & `twikit-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/client.py` & `twikit-1.5.0/twikit/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from functools import partial
 from typing import Literal
 
 import filetype
 from fake_useragent import UserAgent
 from httpx import Response
 
+from .community import Community, CommunityMember
 from .errors import (
     CouldNotTweet,
+    InvalidMedia,
     TweetNotAvailable,
     TwitterException,
     UserNotFound,
     UserUnavailable,
     raise_exceptions_from_response
 )
 from .group import Group, GroupMessage
@@ -24,15 +26,17 @@
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet
 from .user import User
 from .utils import (
+    COMMUNITY_TWEETS_FEATURES,
     COMMUNITY_NOTE_FEATURES,
+    JOIN_COMMUNITY_FEATURES,
     LIST_FEATURES,
     FEATURES,
     TOKEN,
     USER_FEATURES,
     Endpoint,
     Flow,
     Result,
@@ -698,15 +702,18 @@
             params=params,
             headers=self._base_headers,
         )
 
         if wait_for_completion:
             while True:
                 state = self.check_media_status(media_id)
-                if state['processing_info']['state'] == 'succeeded':
+                processing_info = state['processing_info']
+                if 'error' in processing_info:
+                    raise InvalidMedia(processing_info['error'].get('message'))
+                if processing_info['state'] == 'succeeded':
                     break
                 time.sleep(status_check_interval)
 
         return media_id
 
     def check_media_status(self, media_id: str) -> dict:
         """
@@ -775,14 +782,24 @@
             data['sensitive_media_warning'] = sensitive_warning
         return self.http.post(
             Endpoint.CREATE_MEDIA_METADATA,
             json=data,
             headers=self._base_headers
         )
 
+    def get_media(self, url: str) -> bytes:
+        """Retrieves media bytes.
+
+        Parameters
+        ----------
+        url : str
+            Media URL
+        """
+        return self.http.get(url, headers=self._base_headers).content
+
     def create_poll(
         self,
         choices: list[str],
         duration_minutes: int
     ) -> str:
         """
         Creates a poll and returns card-uri.
@@ -3615,14 +3632,63 @@
         return self._get_list_users(
             Endpoint.LIST_SUBSCRIBERS,
             list_id,
             count,
             cursor
         )
 
+    def search_list(
+        self, query: str, count: int = 20, cursor: str | None = None
+    ) -> Result[List]:
+        """
+        Search for lists based on the provided query.
+
+        Parameters
+        ----------
+        query : :class:`str`
+            The search query.
+        count : :class:`int`, default=20
+            The number of lists to retrieve.
+
+        Returns
+        -------
+        Result[:class:`List`]
+            An instance of the `Result` class containing the
+            search results.
+
+        Examples
+        --------
+        >>> lists = client.search_list('query')
+        >>> for list in lists:
+        ...     print(list)
+        <List id="...">
+        <List id="...">
+        ...
+
+        >>> more_lists = lists.next()  # Retrieve more lists
+        """
+        response = self._search(query, 'Lists', count, cursor)
+        entries = find_dict(response, 'entries')[0]
+
+        if cursor is None:
+            items = entries[0]['content']['items']
+        else:
+            items = find_dict(response, 'moduleItems')[0]
+
+        lists = []
+        for item in items:
+            lists.append(List(self, item['item']['itemContent']['list']))
+        next_cursor = entries[-1]['content']['value']
+
+        return Result(
+            lists,
+            partial(self.search_list, query, count, next_cursor),
+            next_cursor
+        )
+
     def get_notifications(
         self,
         type: Literal['All', 'Verified', 'Mentions'],
         count: int = 40,
         cursor: str | None = None
     ) -> Result[Notification]:
         """
@@ -3720,7 +3786,526 @@
             next_cursor = None
 
         return Result(
             notifications,
             partial(self.get_notifications, type, count, next_cursor),
             next_cursor
         )
+
+    def search_community(
+        self, query: str, cursor: str | None = None
+    ) -> Result[Community]:
+        """
+        Searchs communities based on the specified query.
+
+        Parameters
+        ----------
+        query : :class:`str`
+            The search query.
+
+        Returns
+        -------
+        Result[:class:`Community`]
+            List of retrieved communities.
+
+        Examples
+        --------
+        >>> communities = client.search_communities('query')
+        >>> for community in communities:
+        ...     print(community)
+        <Community id="...">
+        <Community id="...">
+        ...
+
+        >>> more_communities = communities.next()  # Retrieve more communities
+        """
+        variables = {
+            'query': query,
+        }
+        if cursor is not None:
+            variables['cursor'] = cursor
+        params = flatten_params({
+            'variables': variables
+        })
+        response = self.http.get(
+            Endpoint.SEARCH_COMMUNITY,
+            params=params,
+            headers=self._base_headers
+        ).json()
+
+        items = find_dict(response, 'items_results')[0]
+        communities = []
+        for item in items:
+            communities.append(Community(self, item['result']))
+        next_cursor_ = find_dict(response, 'next_cursor')
+        next_cursor = next_cursor_[0] if next_cursor_ else None
+        if next_cursor is None:
+            fetch_next_result = None
+        else:
+            fetch_next_result = partial(self.search_community,
+                                        query, next_cursor)
+        return Result(
+            communities,
+            fetch_next_result,
+            next_cursor
+        )
+
+    def get_community(self, community_id: str) -> Community:
+        """
+        Retrieves community by ID.
+
+        Parameters
+        ----------
+        list_id : :class:`str`
+            The ID of the community to retrieve.
+
+        Returns
+        -------
+        :class:`Community`
+            Community object.
+        """
+        params = flatten_params({
+            'variables': {'communityId': community_id},
+            'features': {
+                'c9s_list_members_action_api_enabled':False,
+                'c9s_superc9s_indication_enabled':False
+            }
+        })
+        response = self.http.get(
+            Endpoint.GET_COMMUNITY,
+            params=params,
+            headers=self._base_headers
+        ).json()
+        community_data = find_dict(response, 'result')[0]
+        return Community(self, community_data)
+
+    def get_community_tweets(
+        self,
+        community_id: str,
+        tweet_type: Literal['Top', 'Latest', 'Media'],
+        count: int = 40,
+        cursor: str | None = None
+    ) -> Result[Tweet]:
+        """
+        Retrieves tweets from a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community.
+        tweet_type : {'Top', 'Latest', 'Media'}
+            The type of tweets to retrieve.
+        count : :class:`int`, default=40
+            The number of tweets to retrieve.
+
+        Returns
+        -------
+        Result[:class:`Tweet`]
+            List of retrieved tweets.
+
+        Examples
+        --------
+        >>> community_id = '...'
+        >>> tweets = client.get_community_tweets(community_id, 'Latest')
+        >>> for tweet in tweets:
+        ...     print(tweet)
+        <Tweet id="...">
+        <Tweet id="...">
+        ...
+        >>> more_tweets = tweets.next()  # Retrieve more tweets
+        """
+        tweet_type = tweet_type.capitalize()
+
+        variables = {
+            'communityId': community_id,
+            'count': count,
+            'withCommunity': True
+        }
+
+        if tweet_type == 'Media':
+            endpoint = Endpoint.COMMUNITY_MEDIA
+        else:
+            endpoint = Endpoint.COMMUNITY_TWEETS
+            variables['rankingMode'] = {
+                'Top': 'Relevance',
+                'Latest': 'Recency'
+            }[tweet_type]
+
+        if cursor is not None:
+            variables['cursor'] = cursor
+
+        params = flatten_params({
+            'variables': variables,
+            'features': COMMUNITY_TWEETS_FEATURES
+        })
+        response = self.http.get(
+            endpoint,
+            params=params,
+            headers=self._base_headers
+        ).json()
+
+        entries = find_dict(response, 'entries')[0]
+        if tweet_type == 'Media':
+            if cursor is None:
+                items = entries[0]['content']['items']
+                next_cursor = entries[-1]['content']['value']
+                previous_cursor = entries[-2]['content']['value']
+            else:
+                items = find_dict(response, 'moduleItems')[0]
+                next_cursor = entries[-1]['content']['value']
+                previous_cursor = entries[-2]['content']['value']
+        else:
+            items = entries
+            next_cursor = items[-1]['content']['value']
+            previous_cursor = items[-2]['content']['value']
+
+        tweets = []
+        for item in items:
+            if not item['entryId'].startswith(('tweet', 'communities-grid')):
+                continue
+            tweet_data = find_dict(item, 'result')[0]
+            if 'tweet' in tweet_data:
+                tweet_data = tweet_data['tweet']
+            user_data = tweet_data['core']['user_results']['result']
+            tweets.append(Tweet(self, tweet_data, User(self, user_data)))
+
+        return Result(
+            tweets,
+            partial(self.get_community_tweets, community_id,
+                    tweet_type, count, next_cursor),
+            next_cursor,
+            partial(self.get_community_tweets, community_id,
+                    tweet_type, count, previous_cursor),
+            previous_cursor
+        )
+
+    def get_communities_timeline(
+        self, count: int = 20, cursor: str | None = None
+    ) -> Result[Tweet]:
+        """
+        Retrieves tweets from communities timeline.
+
+        Parameters
+        ----------
+        count : :class:`int`, default=20
+            The number of tweets to retrieve.
+
+        Returns
+        -------
+        Result[:class:`Tweet`]
+            List of retrieved tweets.
+
+        Examples
+        --------
+        >>> tweets = client.get_communities_timeline()
+        >>> for tweet in tweets:
+        ...     print(tweet)
+        <Tweet id="...">
+        <Tweet id="...">
+        ...
+        >>> more_tweets = tweets.next()  # Retrieve more tweets
+        """
+        variables = {
+            'count': count,
+            'withCommunity': True
+        }
+        if cursor is not None:
+            variables['cursor'] = cursor
+        params = flatten_params({
+            'variables': variables,
+            'features': COMMUNITY_TWEETS_FEATURES
+        })
+        response = self.http.get(
+            Endpoint.COMMUNITIES_TIMELINE,
+            params=params,
+            headers=self._base_headers
+        ).json()
+        items = find_dict(response, 'entries')[0]
+        tweets = []
+        for item in items:
+            if not item['entryId'].startswith('tweet'):
+                continue
+            tweet_data = find_dict(item, 'result')[0]
+            if 'tweet' in tweet_data:
+                tweet_data = tweet_data['tweet']
+            user_data = tweet_data['core']['user_results']['result']
+            community_data = tweet_data['community_results']['result']
+            community_data['rest_id'] = community_data['id_str']
+            community = Community(self, community_data)
+            tweet = Tweet(
+                self, tweet_data, User(self, user_data)
+            )
+            tweet.community = community
+            tweets.append(tweet)
+
+        next_cursor = items[-1]['content']['value']
+        previous_cursor = items[-2]['content']['value']
+
+        return Result(
+            tweets,
+            partial(self.get_communities_timeline, count, next_cursor),
+            next_cursor,
+            partial(self.get_communities_timeline, count, previous_cursor),
+            previous_cursor
+        )
+
+    def join_community(self, community_id: str) -> Community:
+        """
+        Join a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community to join.
+
+        Returns
+        -------
+        :class:`Community`
+            The joined community.
+        """
+        data = {
+            'variables': {
+                'communityId': community_id
+            },
+            'features': JOIN_COMMUNITY_FEATURES,
+            'queryId': get_query_id(Endpoint.JOIN_COMMUNITY)
+        }
+        response = self.http.post(
+            Endpoint.JOIN_COMMUNITY,
+            json=data,
+            headers=self._base_headers
+        ).json()
+        community_data = response['data']['community_join']
+        community_data['rest_id'] = community_data['id_str']
+        return Community(self, community_data)
+
+    def leave_community(self, community_id: str) -> Community:
+        """
+        Leave a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community to leave.
+
+        Returns
+        -------
+        :class:`Community`
+            The left community.
+        """
+        data = {
+            'variables': {
+                'communityId': community_id
+            },
+            'features': JOIN_COMMUNITY_FEATURES,
+            'queryId': get_query_id(Endpoint.LEAVE_COMMUNITY)
+        }
+        response = self.http.post(
+            Endpoint.LEAVE_COMMUNITY,
+            json=data,
+            headers=self._base_headers
+        ).json()
+        community_data = response['data']['community_leave']
+        community_data['rest_id'] = community_data['id_str']
+        return Community(self, community_data)
+
+    def request_to_join_community(
+        self, community_id: str, answer: str | None = None
+    ) -> Community:
+        """
+        Request to join a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community to request to join.
+        answer : :class:`str`, default=None
+            The answer to the join request.
+
+        Returns
+        -------
+        :class:`Community`
+            The requested community.
+        """
+        data = {
+            'variables': {
+                'communityId': community_id,
+                'answer': '' if answer is None else answer
+            },
+            'features': JOIN_COMMUNITY_FEATURES,
+            'queryId': get_query_id(Endpoint.REQUEST_TO_JOIN_COMMUNITY)
+        }
+        response = self.http.post(
+            Endpoint.REQUEST_TO_JOIN_COMMUNITY,
+            json=data,
+            headers=self._base_headers
+        ).json()
+        community_data = find_dict(response, 'result')[0]
+        community_data['rest_id'] = community_data['id_str']
+        return Community(self, community_data)
+
+    def _get_community_users(
+        self, endpoint: str, community_id: str, count: int, cursor: str | None
+    ):
+        """
+        Base function to retrieve community users.
+        """
+        variables = {
+            'communityId': community_id,
+            'count': count
+        }
+        if cursor is not None:
+            variables['cursor'] = cursor
+        params = flatten_params({
+            'variables': variables,
+            'features': {
+                'responsive_web_graphql_timeline_navigation_enabled': True
+            }
+        })
+        response =  self.http.get(
+            endpoint,
+            params=params,
+            headers=self._base_headers
+        ).json()
+
+        items = find_dict(response, 'items_results')[0]
+        users = []
+        for item in items:
+            if not 'result' in item:
+                continue
+            if item['result'].get('__typename') != 'User':
+                continue
+            users.append(CommunityMember(self, item['result']))
+
+        next_cursor_ = find_dict(response, 'next_cursor')
+        next_cursor = next_cursor_[0] if next_cursor_ else None
+
+        if next_cursor is None:
+            fetch_next_result = None
+        else:
+            fetch_next_result = partial(self._get_community_users, endpoint,
+                                        community_id, count, next_cursor)
+        return Result(
+            users,
+            fetch_next_result,
+            next_cursor
+        )
+
+    def get_community_members(
+        self, community_id: str, count: int = 20, cursor: str | None = None
+    ) -> Result[CommunityMember]:
+        """
+        Retrieves members of a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community.
+        count : :class:`int`, default=20
+            The number of members to retrieve.
+
+        Returns
+        -------
+        Result[:class:`CommunityMember`]
+            List of retrieved members.
+        """
+        return self._get_community_users(
+            Endpoint.COMMUNITY_MEMBERS,
+            community_id,
+            count,
+            cursor
+        )
+
+    def get_community_moderators(
+        self, community_id: str, count: int = 20, cursor: str | None = None
+    ) -> Result[CommunityMember]:
+        """
+        Retrieves moderators of a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community.
+        count : :class:`int`, default=20
+            The number of moderators to retrieve.
+
+        Returns
+        -------
+        Result[:class:`CommunityMember`]
+            List of retrieved moderators.
+        """
+        return self._get_community_users(
+            Endpoint.COMMUNITY_MODERATORS,
+            community_id,
+            count,
+            cursor
+        )
+
+    def search_community_tweet(
+        self,
+        community_id: str,
+        query: str,
+        count: int = 20,
+        cursor: str | None = None
+    ) -> Result[Tweet]:
+        """Searchs tweets in a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community.
+        query : :class:`str`
+            The search query.
+        count : :class:`int`, default=20
+            The number of tweets to retrieve.
+
+        Returns
+        -------
+        Result[:class:`Tweet`]
+            List of retrieved tweets.
+        """
+        variables = {
+            "count": count,
+            "query": query,
+            "communityId": community_id,
+            "includePromotedContent": False,
+            "withBirdwatchNotes": True,
+            "withVoice": False,
+            "isListMemberTargetUserId": "0",
+            "withCommunity": False,
+            "withSafetyModeUserFields": True
+        }
+        if cursor is not None:
+            variables['cursor'] = cursor
+        params = flatten_params({
+            'variables': variables,
+            'features': COMMUNITY_TWEETS_FEATURES
+        })
+        response = self.http.get(
+            Endpoint.SEARCH_COMMUNITY_TWEET,
+            params=params,
+            headers=self._base_headers
+        ).json()
+
+        items = find_dict(response, 'entries')[0]
+        tweets = []
+        for item in items:
+            if not item['entryId'].startswith('tweet'):
+                continue
+            tweet_data = find_dict(item, 'result')[0]
+            if 'tweet' in tweet_data:
+                tweet_data = tweet_data['tweet']
+            user_data = find_dict(tweet_data, 'result')[0]
+            tweets.append(Tweet(self, tweet_data, User(self, user_data)))
+
+        next_cursor = items[-1]['content']['value']
+        previous_cursor = items[-2]['content']['value']
+
+        return Result(
+            tweets,
+            partial(self.search_community_tweet, community_id,
+                    query, count, next_cursor),
+            next_cursor,
+            partial(self.search_community_tweet, community_id,
+                    query, count, previous_cursor),
+            previous_cursor,
+        )
```

### Comparing `twikit-1.4.9/twikit/errors.py` & `twikit-1.5.0/twikit/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 class TwitterException(Exception):
     """
     Base class for Twitter API related exceptions.
     """
+    def __init__(self, *args: object, headers: dict | None = None) -> None:
+        super().__init__(*args)
+        if headers is None:
+            self.headers = None
+        else:
+            self.headers = dict(headers)
 
 class BadRequest(TwitterException):
     """
     Exception raised for 400 Bad Request errors.
     """
 
 class Unauthorized(TwitterException):
@@ -29,15 +35,15 @@
     """
 
 class TooManyRequests(TwitterException):
     """
     Exception raised for 429 Too Many Requests errors.
     """
     def __init__(self, *args, headers: dict | None = None) -> None:
-        super().__init__(*args)
+        super().__init__(*args, headers=headers)
         if headers is not None and 'x-rate-limit-reset' in headers:
             self.rate_limit_reset = int(headers.get('x-rate-limit-reset'))
         else:
             self.rate_limit_reset = None
 
 class ServerError(TwitterException):
     """
```

### Comparing `twikit-1.4.9/twikit/group.py` & `twikit-1.5.0/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/list.py` & `twikit-1.5.0/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/message.py` & `twikit-1.5.0/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/notification.py` & `twikit-1.5.0/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/trend.py` & `twikit-1.5.0/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/tweet.py` & `twikit-1.5.0/twikit/tweet.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .user import User
 from .utils import find_dict, timestamp_to_datetime
 
 if TYPE_CHECKING:
     from httpx import Response
 
     from .client import Client
+    from .community import Community
     from .utils import Result
 
 
 class Tweet:
     """
     Attributes
     ----------
```

### Comparing `twikit-1.4.9/twikit/twikit_async/client.py` & `twikit-1.5.0/twikit/twikit_async/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,34 +9,38 @@
 
 import filetype
 from fake_useragent import UserAgent
 from httpx import Response
 
 from ..errors import (
     CouldNotTweet,
+    InvalidMedia,
     TweetNotAvailable,
     TwitterException,
     UserNotFound,
     UserUnavailable,
     raise_exceptions_from_response
 )
 from ..utils import (
+    COMMUNITY_TWEETS_FEATURES,
     COMMUNITY_NOTE_FEATURES,
     FEATURES,
+    JOIN_COMMUNITY_FEATURES,
     LIST_FEATURES,
     TOKEN,
     USER_FEATURES,
     Endpoint,
     build_tweet_data,
     build_user_data,
     find_dict,
     flatten_params,
     get_query_id,
     urlencode
 )
+from .community import CommunityRule, Community, CommunityCreator, CommunityMember
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet
@@ -710,16 +714,19 @@
             Endpoint.UPLOAD_MEDIA,
             params=params,
             headers=self._base_headers,
         )
 
         if wait_for_completion:
             while True:
-                state = await self.check_media_status(media_id)
-                if state['processing_info']['state'] == 'succeeded':
+                state = self.check_media_status(media_id)
+                processing_info = state['processing_info']
+                if 'error' in processing_info:
+                    raise InvalidMedia(processing_info['error'].get('message'))
+                if processing_info['state'] == 'succeeded':
                     break
                 await asyncio.sleep(status_check_interval)
 
         return media_id
 
     async def check_media_status(self, media_id: str) -> dict:
         """
@@ -788,14 +795,24 @@
             data['sensitive_media_warning'] = sensitive_warning
         return await self.http.post(
             Endpoint.CREATE_MEDIA_METADATA,
             json=data,
             headers=self._base_headers
         )
 
+    async def get_media(self, url: str) -> bytes:
+        """Retrieves media bytes.
+
+        Parameters
+        ----------
+        url : str
+            Media URL
+        """
+        return (await self.http.get(url, headers=self._base_headers)).content
+
     async def create_poll(
         self,
         choices: list[str],
         duration_minutes: int
     ) -> str:
         """
         Creates a poll and returns card-uri.
@@ -2504,15 +2521,15 @@
         return Result(
             results,
             partial(self._get_user_friendship,
                     user_id, count, endpoint, next_cursor),
             next_cursor
         )
 
-    def get_user_followers(
+    async def get_user_followers(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of followers for a given user.
 
         Parameters
         ----------
@@ -2522,22 +2539,22 @@
             The number of followers to retrieve.
 
         Returns
         -------
         Result[:class:`User`]
             A list of User objects representing the followers.
         """
-        return self._get_user_friendship(
+        return await self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWERS,
             cursor
         )
 
-    def get_user_verified_followers(
+    async def get_user_verified_followers(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of verified followers for a given user.
 
         Parameters
         ----------
@@ -2547,22 +2564,22 @@
             The number of verified followers to retrieve.
 
         Returns
         -------
         Result[:class:`User`]
             A list of User objects representing the verified followers.
         """
-        return self._get_user_friendship(
+        return await self._get_user_friendship(
             user_id,
             count,
             Endpoint.BLUE_VERIFIED_FOLLOWERS,
             cursor
         )
 
-    def get_user_followers_you_know(
+    async def get_user_followers_you_know(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of common followers.
 
         Parameters
         ----------
@@ -2572,22 +2589,22 @@
             The number of followers you might know to retrieve.
 
         Returns
         -------
         Result[:class:`User`]
             A list of User objects representing the followers you might know.
         """
-        return self._get_user_friendship(
+        return await self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWERS_YOU_KNOW,
             cursor
         )
 
-    def get_user_following(
+    async def get_user_following(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of users whom the given user is following.
 
         Parameters
         ----------
@@ -2597,22 +2614,22 @@
             The number of following users to retrieve.
 
         Returns
         -------
         Result[:class:`User`]
             A list of User objects representing the users being followed.
         """
-        return self._get_user_friendship(
+        return await self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWING,
             cursor
         )
 
-    def get_user_subscriptions(
+    async def get_user_subscriptions(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of users to which the specified user is subscribed.
 
         Parameters
         ----------
@@ -2622,15 +2639,15 @@
             The number of subscriptions to retrieve.
 
         Returns
         -------
         Result[:class:`User`]
             A list of User objects representing the subscribed users.
         """
-        return self._get_user_friendship(
+        return await self._get_user_friendship(
             user_id,
             count,
             Endpoint.SUBSCRIPTIONS,
             cursor
         )
 
     async def _send_dm(
@@ -3640,14 +3657,63 @@
         return await self._get_list_users(
             Endpoint.LIST_SUBSCRIBERS,
             list_id,
             count,
             cursor
         )
 
+    async def search_list(
+        self, query: str, count: int = 20, cursor: str | None = None
+    ) -> Result[List]:
+        """
+        Search for lists based on the provided query.
+
+        Parameters
+        ----------
+        query : :class:`str`
+            The search query.
+        count : :class:`int`, default=20
+            The number of lists to retrieve.
+
+        Returns
+        -------
+        Result[:class:`List`]
+            An instance of the `Result` class containing the
+            search results.
+
+        Examples
+        --------
+        >>> lists = await client.search_list('query')
+        >>> for list in lists:
+        ...     print(list)
+        <List id="...">
+        <List id="...">
+        ...
+
+        >>> more_lists = await lists.next()  # Retrieve more lists
+        """
+        response = await self._search(query, 'Lists', count, cursor)
+        entries = find_dict(response, 'entries')[0]
+
+        if cursor is None:
+            items = entries[0]['content']['items']
+        else:
+            items = find_dict(response, 'moduleItems')[0]
+
+        lists = []
+        for item in items:
+            lists.append(List(self, item['item']['itemContent']['list']))
+        next_cursor = entries[-1]['content']['value']
+
+        return Result(
+            lists,
+            partial(self.search_list, query, count, next_cursor),
+            next_cursor
+        )
+
     async def get_notifications(
         self,
         type: Literal['All', 'Verified', 'Mentions'],
         count: int = 40,
         cursor: str | None = None
     ) -> Result[Notification]:
         """
@@ -3745,7 +3811,527 @@
             next_cursor = None
 
         return Result(
             notifications,
             partial(self.get_notifications, type, count, next_cursor),
             next_cursor
         )
+
+    async def search_community(
+        self, query: str, cursor: str | None = None
+    ) -> Result[Community]:
+        """
+        Searchs communities based on the specified query.
+
+        Parameters
+        ----------
+        query : :class:`str`
+            The search query.
+
+        Returns
+        -------
+        Result[:class:`Community`]
+            List of retrieved communities.
+
+        Examples
+        --------
+        >>> communities = await client.search_communities('query')
+        >>> for community in communities:
+        ...     print(community)
+        <Community id="...">
+        <Community id="...">
+        ...
+
+        >>> # Retrieve more communities
+        >>> more_communities = await communities.next()
+        """
+        variables = {
+            'query': query,
+        }
+        if cursor is not None:
+            variables['cursor'] = cursor
+        params = flatten_params({
+            'variables': variables
+        })
+        response = (await self.http.get(
+            Endpoint.SEARCH_COMMUNITY,
+            params=params,
+            headers=self._base_headers
+        )).json()
+
+        items = find_dict(response, 'items_results')[0]
+        communities = []
+        for item in items:
+            communities.append(Community(self, item['result']))
+        next_cursor_ = find_dict(response, 'next_cursor')
+        next_cursor = next_cursor_[0] if next_cursor_ else None
+        if next_cursor is None:
+            fetch_next_result = None
+        else:
+            fetch_next_result = partial(self.search_community,
+                                        query, next_cursor)
+        return Result(
+            communities,
+            fetch_next_result,
+            next_cursor
+        )
+
+    async def get_community(self, community_id: str) -> Community:
+        """
+        Retrieves community by ID.
+
+        Parameters
+        ----------
+        list_id : :class:`str`
+            The ID of the community to retrieve.
+
+        Returns
+        -------
+        :class:`Community`
+            Community object.
+        """
+        params = flatten_params({
+            'variables': {'communityId': community_id},
+            'features': {
+                'c9s_list_members_action_api_enabled':False,
+                'c9s_superc9s_indication_enabled':False
+            }
+        })
+        response = (await self.http.get(
+            Endpoint.GET_COMMUNITY,
+            params=params,
+            headers=self._base_headers
+        )).json()
+        community_data = find_dict(response, 'result')[0]
+        return Community(self, community_data)
+
+    async def get_community_tweets(
+        self,
+        community_id: str,
+        tweet_type: Literal['Top', 'Latest', 'Media'],
+        count: int = 40,
+        cursor: str | None = None
+    ) -> Result[Tweet]:
+        """
+        Retrieves tweets from a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community.
+        tweet_type : {'Top', 'Latest', 'Media'}
+            The type of tweets to retrieve.
+        count : :class:`int`, default=40
+            The number of tweets to retrieve.
+
+        Returns
+        -------
+        Result[:class:`Tweet`]
+            List of retrieved tweets.
+
+        Examples
+        --------
+        >>> community_id = '...'
+        >>> tweets = await client.get_community_tweets(community_id, 'Latest')
+        >>> for tweet in tweets:
+        ...     print(tweet)
+        <Tweet id="...">
+        <Tweet id="...">
+        ...
+        >>> more_tweets = await tweets.next()  # Retrieve more tweets
+        """
+        tweet_type = tweet_type.capitalize()
+
+        variables = {
+            'communityId': community_id,
+            'count': count,
+            'withCommunity': True
+        }
+
+        if tweet_type == 'Media':
+            endpoint = Endpoint.COMMUNITY_MEDIA
+        else:
+            endpoint = Endpoint.COMMUNITY_TWEETS
+            variables['rankingMode'] = {
+                'Top': 'Relevance',
+                'Latest': 'Recency'
+            }[tweet_type]
+
+        if cursor is not None:
+            variables['cursor'] = cursor
+
+        params = flatten_params({
+            'variables': variables,
+            'features': COMMUNITY_TWEETS_FEATURES
+        })
+        response = (await self.http.get(
+            endpoint,
+            params=params,
+            headers=self._base_headers
+        )).json()
+
+        entries = find_dict(response, 'entries')[0]
+        if tweet_type == 'Media':
+            if cursor is None:
+                items = entries[0]['content']['items']
+                next_cursor = entries[-1]['content']['value']
+                previous_cursor = entries[-2]['content']['value']
+            else:
+                items = find_dict(response, 'moduleItems')[0]
+                next_cursor = entries[-1]['content']['value']
+                previous_cursor = entries[-2]['content']['value']
+        else:
+            items = entries
+            next_cursor = items[-1]['content']['value']
+            previous_cursor = items[-2]['content']['value']
+
+        tweets = []
+        for item in items:
+            if not item['entryId'].startswith(('tweet', 'communities-grid')):
+                continue
+            tweet_data = find_dict(item, 'result')[0]
+            if 'tweet' in tweet_data:
+                tweet_data = tweet_data['tweet']
+            user_data = tweet_data['core']['user_results']['result']
+            tweets.append(Tweet(self, tweet_data, User(self, user_data)))
+
+        return Result(
+            tweets,
+            partial(self.get_community_tweets, community_id,
+                    tweet_type, count, next_cursor),
+            next_cursor,
+            partial(self.get_community_tweets, community_id,
+                    tweet_type, count, previous_cursor),
+            previous_cursor
+        )
+
+    async def get_communities_timeline(
+        self, count: int = 20, cursor: str | None = None
+    ) -> Result[Tweet]:
+        """
+        Retrieves tweets from communities timeline.
+
+        Parameters
+        ----------
+        count : :class:`int`, default=20
+            The number of tweets to retrieve.
+
+        Returns
+        -------
+        Result[:class:`Tweet`]
+            List of retrieved tweets.
+
+        Examples
+        --------
+        >>> tweets = await client.get_communities_timeline()
+        >>> for tweet in tweets:
+        ...     print(tweet)
+        <Tweet id="...">
+        <Tweet id="...">
+        ...
+        >>> more_tweets = await tweets.next()  # Retrieve more tweets
+        """
+        variables = {
+            'count': count,
+            'withCommunity': True
+        }
+        if cursor is not None:
+            variables['cursor'] = cursor
+        params = flatten_params({
+            'variables': variables,
+            'features': COMMUNITY_TWEETS_FEATURES
+        })
+        response = (await self.http.get(
+            Endpoint.COMMUNITIES_TIMELINE,
+            params=params,
+            headers=self._base_headers
+        )).json()
+        items = find_dict(response, 'entries')[0]
+        tweets = []
+        for item in items:
+            if not item['entryId'].startswith('tweet'):
+                continue
+            tweet_data = find_dict(item, 'result')[0]
+            if 'tweet' in tweet_data:
+                tweet_data = tweet_data['tweet']
+            user_data = tweet_data['core']['user_results']['result']
+            community_data = tweet_data['community_results']['result']
+            community_data['rest_id'] = community_data['id_str']
+            community = Community(self, community_data)
+            tweet = Tweet(
+                self, tweet_data, User(self, user_data)
+            )
+            tweet.community = community
+            tweets.append(tweet)
+
+        next_cursor = items[-1]['content']['value']
+        previous_cursor = items[-2]['content']['value']
+
+        return Result(
+            tweets,
+            partial(self.get_communities_timeline, count, next_cursor),
+            next_cursor,
+            partial(self.get_communities_timeline, count, previous_cursor),
+            previous_cursor
+        )
+
+    async def join_community(self, community_id: str) -> Community:
+        """
+        Join a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community to join.
+
+        Returns
+        -------
+        :class:`Community`
+            The joined community.
+        """
+        data = {
+            'variables': {
+                'communityId': community_id
+            },
+            'features': JOIN_COMMUNITY_FEATURES,
+            'queryId': get_query_id(Endpoint.JOIN_COMMUNITY)
+        }
+        response = (await self.http.post(
+            Endpoint.JOIN_COMMUNITY,
+            json=data,
+            headers=self._base_headers
+        )).json()
+        community_data = response['data']['community_join']
+        community_data['rest_id'] = community_data['id_str']
+        return Community(self, community_data)
+
+    async def leave_community(self, community_id: str) -> Community:
+        """
+        Leave a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community to leave.
+
+        Returns
+        -------
+        :class:`Community`
+            The left community.
+        """
+        data = {
+            'variables': {
+                'communityId': community_id
+            },
+            'features': JOIN_COMMUNITY_FEATURES,
+            'queryId': get_query_id(Endpoint.LEAVE_COMMUNITY)
+        }
+        response = (await self.http.post(
+            Endpoint.LEAVE_COMMUNITY,
+            json=data,
+            headers=self._base_headers
+        )).json()
+        community_data = response['data']['community_leave']
+        community_data['rest_id'] = community_data['id_str']
+        return Community(self, community_data)
+
+    async def request_to_join_community(
+        self, community_id: str, answer: str | None = None
+    ) -> Community:
+        """
+        Request to join a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community to request to join.
+        answer : :class:`str`, default=None
+            The answer to the join request.
+
+        Returns
+        -------
+        :class:`Community`
+            The requested community.
+        """
+        data = {
+            'variables': {
+                'communityId': community_id,
+                'answer': '' if answer is None else answer
+            },
+            'features': JOIN_COMMUNITY_FEATURES,
+            'queryId': get_query_id(Endpoint.REQUEST_TO_JOIN_COMMUNITY)
+        }
+        response = (await self.http.post(
+            Endpoint.REQUEST_TO_JOIN_COMMUNITY,
+            json=data,
+            headers=self._base_headers
+        )).json()
+        community_data = find_dict(response, 'result')[0]
+        community_data['rest_id'] = community_data['id_str']
+        return Community(self, community_data)
+
+    async def _get_community_users(
+        self, endpoint: str, community_id: str, count: int, cursor: str | None
+    ):
+        """
+        Base function to retrieve community users.
+        """
+        variables = {
+            'communityId': community_id,
+            'count': count
+        }
+        if cursor is not None:
+            variables['cursor'] = cursor
+        params = flatten_params({
+            'variables': variables,
+            'features': {
+                'responsive_web_graphql_timeline_navigation_enabled': True
+            }
+        })
+        response = (await self.http.get(
+            endpoint,
+            params=params,
+            headers=self._base_headers
+        )).json()
+
+        items = find_dict(response, 'items_results')[0]
+        users = []
+        for item in items:
+            if not 'result' in item:
+                continue
+            if item['result'].get('__typename') != 'User':
+                continue
+            users.append(CommunityMember(self, item['result']))
+
+        next_cursor_ = find_dict(response, 'next_cursor')
+        next_cursor = next_cursor_[0] if next_cursor_ else None
+
+        if next_cursor is None:
+            fetch_next_result = None
+        else:
+            fetch_next_result = partial(self._get_community_users, endpoint,
+                                        community_id, count, next_cursor)
+        return Result(
+            users,
+            fetch_next_result,
+            next_cursor
+        )
+
+    async def get_community_members(
+        self, community_id: str, count: int = 20, cursor: str | None = None
+    ) -> Result[CommunityMember]:
+        """
+        Retrieves members of a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community.
+        count : :class:`int`, default=20
+            The number of members to retrieve.
+
+        Returns
+        -------
+        Result[:class:`CommunityMember`]
+            List of retrieved members.
+        """
+        return await self._get_community_users(
+            Endpoint.COMMUNITY_MEMBERS,
+            community_id,
+            count,
+            cursor
+        )
+
+    async def get_community_moderators(
+        self, community_id: str, count: int = 20, cursor: str | None = None
+    ) -> Result[CommunityMember]:
+        """
+        Retrieves moderators of a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community.
+        count : :class:`int`, default=20
+            The number of moderators to retrieve.
+
+        Returns
+        -------
+        Result[:class:`CommunityMember`]
+            List of retrieved moderators.
+        """
+        return await self._get_community_users(
+            Endpoint.COMMUNITY_MODERATORS,
+            community_id,
+            count,
+            cursor
+        )
+
+    async def search_community_tweet(
+        self,
+        community_id: str,
+        query: str,
+        count: int = 20,
+        cursor: str | None = None
+    ) -> Result[Tweet]:
+        """Searchs tweets in a community.
+
+        Parameters
+        ----------
+        community_id : :class:`str`
+            The ID of the community.
+        query : :class:`str`
+            The search query.
+        count : :class:`int`, default=20
+            The number of tweets to retrieve.
+
+        Returns
+        -------
+        Result[:class:`Tweet`]
+            List of retrieved tweets.
+        """
+        variables = {
+            "count": count,
+            "query": query,
+            "communityId": community_id,
+            "includePromotedContent": False,
+            "withBirdwatchNotes": True,
+            "withVoice": False,
+            "isListMemberTargetUserId": "0",
+            "withCommunity": False,
+            "withSafetyModeUserFields": True
+        }
+        if cursor is not None:
+            variables['cursor'] = cursor
+        params = flatten_params({
+            'variables': variables,
+            'features': COMMUNITY_TWEETS_FEATURES
+        })
+        response = (await self.http.get(
+            Endpoint.SEARCH_COMMUNITY_TWEET,
+            params=params,
+            headers=self._base_headers
+        )).json()
+
+        items = find_dict(response, 'entries')[0]
+        tweets = []
+        for item in items:
+            if not item['entryId'].startswith('tweet'):
+                continue
+            tweet_data = find_dict(item, 'result')[0]
+            if 'tweet' in tweet_data:
+                tweet_data = tweet_data['tweet']
+            user_data = find_dict(tweet_data, 'result')[0]
+            tweets.append(Tweet(self, tweet_data, User(self, user_data)))
+
+        next_cursor = items[-1]['content']['value']
+        previous_cursor = items[-2]['content']['value']
+
+        return Result(
+            tweets,
+            partial(self.search_community_tweet, community_id,
+                    query, count, next_cursor),
+            next_cursor,
+            partial(self.search_community_tweet, community_id,
+                    query, count, previous_cursor),
+            previous_cursor,
+        )
```

### Comparing `twikit-1.4.9/twikit/twikit_async/errors.py` & `twikit-1.5.0/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/twikit_async/group.py` & `twikit-1.5.0/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/twikit_async/list.py` & `twikit-1.5.0/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/twikit_async/message.py` & `twikit-1.5.0/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/twikit_async/notification.py` & `twikit-1.5.0/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/twikit_async/trend.py` & `twikit-1.5.0/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/twikit_async/tweet.py` & `twikit-1.5.0/twikit/twikit_async/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,14 +432,30 @@
         """
         return await self._client.delete_scheduled_tweet(self.id)
 
     def __repr__(self) -> str:
         return f'<ScheduledTweet id="{self.id}">'
 
 
+class TweetTombstone:
+    def __init__(self, client: Client, tweet_id: str, data: dict) -> None:
+        self._client = client
+        self.id = tweet_id
+        self.text: str = data['text']['text']
+
+    def __repr__(self) -> str:
+        return f'<TweetTombstone id="{self.id}">'
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, TweetTombstone) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self == __value
+
+
 class Poll:
     """Represents a poll associated with a tweet.
     Attributes
     ----------
     tweet : :class:`Tweet`
         The tweet associated with the poll.
     id : :class:`str`
```

### Comparing `twikit-1.4.9/twikit/twikit_async/user.py` & `twikit-1.5.0/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/twikit_async/utils.py` & `twikit-1.5.0/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/user.py` & `twikit-1.5.0/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.9/twikit/utils.py` & `twikit-1.5.0/twikit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import base64
 import json
 from datetime import datetime
 from typing import (
     Any,
     TYPE_CHECKING,
     Callable,
     Generic,
@@ -70,14 +71,48 @@
     'responsive_web_graphql_timeline_navigation_enabled': True,
     'rweb_tipjar_consumption_enabled': False,
     'responsive_web_graphql_exclude_directive_enabled': True,
     'verified_phone_label_enabled': False,
     'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False
 }
 
+COMMUNITY_TWEETS_FEATURES = {
+    'rweb_tipjar_consumption_enabled': True,
+    'responsive_web_graphql_exclude_directive_enabled': True,
+    'verified_phone_label_enabled': False,
+    'creator_subscriptions_tweet_preview_api_enabled': True,
+    'responsive_web_graphql_timeline_navigation_enabled': True,
+    'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+    'communities_web_enable_tweet_community_results_fetch': True,
+    'c9s_tweet_anatomy_moderator_badge_enabled': True,
+    'tweetypie_unmention_optimization_enabled': True,
+    'responsive_web_edit_tweet_api_enabled': True,
+    'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
+    'view_counts_everywhere_api_enabled': True,
+    'longform_notetweets_consumption_enabled': True,
+    'responsive_web_twitter_article_tweet_consumption_enabled': True,
+    'tweet_awards_web_tipping_enabled': False,
+    'creator_subscriptions_quote_tweet_preview_enabled': False,
+    'freedom_of_speech_not_reach_fetch_enabled': True,
+    'standardized_nudges_misinfo': True,
+    'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': True,
+    'rweb_video_timestamps_enabled': True,
+    'longform_notetweets_rich_text_read_enabled': True,
+    'longform_notetweets_inline_media_enabled': True,
+    'responsive_web_enhance_cards_enabled': False
+}
+
+JOIN_COMMUNITY_FEATURES = {
+    'rweb_tipjar_consumption_enabled': True,
+    'responsive_web_graphql_exclude_directive_enabled': True,
+    'verified_phone_label_enabled': False,
+    'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+    'responsive_web_graphql_timeline_navigation_enabled': True
+}
+
 
 class Endpoint:
     """
     A class containing Twitter API endpoints.
     """
     LOGIN_FLOW = 'https://api.twitter.com/1.1/onboarding/task.json'
     LOGOUT = 'https://api.twitter.com/1.1/account/logout.json'
@@ -146,14 +181,25 @@
     LIST_MANAGEMENT = 'https://twitter.com/i/api/graphql/47170qwZCt5aFo9cBwFoNA/ListsManagementPageTimeline'
     NOTIFICATIONS_ALL = 'https://twitter.com/i/api/2/notifications/all.json'
     NOTIFICATIONS_VERIFIED = 'https://twitter.com/i/api/2/notifications/verified.json'
     NOTIFICATIONS_MENTIONES = 'https://twitter.com/i/api/2/notifications/mentions.json'
     VOTE = 'https://caps.twitter.com/v2/capi/passthrough/1'
     REPORT_FLOW = 'https://twitter.com/i/api/1.1/report/flow.json'
     FETCH_COMMUNITY_NOTE = 'https://twitter.com/i/api/graphql/fKWPPj271aTM-AB9Xp48IA/BirdwatchFetchOneNote'
+    SEARCH_COMMUNITY = 'https://twitter.com/i/api/graphql/daVUkhfHn7-Z8llpYVKJSw/CommunitiesSearchQuery'
+    GET_COMMUNITY = 'https://twitter.com/i/api/graphql/lUBKrilodgg9Nikaw3cIiA/CommunityQuery'
+    COMMUNITY_TWEETS = 'https://twitter.com/i/api/graphql/mhwSsmub4JZgHcs0dtsjrw/CommunityTweetsTimeline'
+    COMMUNITY_MEDIA = 'https://twitter.com/i/api/graphql/Ht5K2ckaZYAOuRFmFfbHig/CommunityMediaTimeline'
+    COMMUNITIES_TIMELINE = 'https://twitter.com/i/api/graphql/4-4iuIdaLPpmxKnA3mr2LA/CommunitiesMainPageTimeline'
+    JOIN_COMMUNITY = 'https://twitter.com/i/api/graphql/xZQLbDwbI585YTG0QIpokw/JoinCommunity'
+    REQUEST_TO_JOIN_COMMUNITY = 'https://twitter.com/i/api/graphql/XwWChphD_6g7JnsFus2f2Q/RequestToJoinCommunity'
+    LEAVE_COMMUNITY = 'https://twitter.com/i/api/graphql/OoS6Kd4-noNLXPZYHtygeA/LeaveCommunity'
+    COMMUNITY_MEMBERS = 'https://twitter.com/i/api/graphql/KDAssJ5lafCy-asH4wm1dw/membersSliceTimeline_Query'
+    COMMUNITY_MODERATORS = 'https://twitter.com/i/api/graphql/9KI_r8e-tgp3--N5SZYVjg/moderatorsSliceTimeline_Query'
+    SEARCH_COMMUNITY_TWEET = 'https://twitter.com/i/api/graphql/5341rmzzvdjqfmPKfoHUBw/CommunityTweetSearchModuleQuery'
 
 T = TypeVar('T')
 
 
 class Result(Generic[T]):
     """
     This class is for storing multiple results.
@@ -373,14 +419,19 @@
     flattened_params = {}
     for key, value in params.items():
         if isinstance(value, (list, dict)):
             value = json.dumps(value)
         flattened_params[key] = value
     return flattened_params
 
+
+def b64_to_str(b64: str) -> str:
+    return base64.b64decode(b64).decode()
+
+
 FILTERS = Literal[
     'media',
     'retweets',
     'native_video',
     'periscope',
     'vine',
     'images',
```

### Comparing `twikit-1.4.9/twikit.egg-info/PKG-INFO` & `twikit-1.5.0/twikit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.9
+Version: 1.5.0
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.9/twikit.egg-info/SOURCES.txt` & `twikit-1.5.0/twikit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 twikit/__init__.py
 twikit/client.py
+twikit/community.py
 twikit/errors.py
 twikit/group.py
 twikit/http.py
 twikit/list.py
 twikit/message.py
 twikit/notification.py
 twikit/trend.py
@@ -16,14 +17,15 @@
 twikit.egg-info/PKG-INFO
 twikit.egg-info/SOURCES.txt
 twikit.egg-info/dependency_links.txt
 twikit.egg-info/requires.txt
 twikit.egg-info/top_level.txt
 twikit/twikit_async/__init__.py
 twikit/twikit_async/client.py
+twikit/twikit_async/community.py
 twikit/twikit_async/errors.py
 twikit/twikit_async/group.py
 twikit/twikit_async/http.py
 twikit/twikit_async/list.py
 twikit/twikit_async/message.py
 twikit/twikit_async/notification.py
 twikit/twikit_async/trend.py
```

