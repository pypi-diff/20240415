# Comparing `tmp/tap-linkedin-ads-2.2.0.tar.gz` & `tmp/tap-linkedin-ads-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-linkedin-ads-2.2.0.tar", last modified: Mon Apr  8 17:48:54 2024, max compression
+gzip compressed data, was "dist/tap-linkedin-ads-2.3.0.tar", last modified: Mon Apr 15 10:01:00 2024, max compression
```

## Comparing `tap-linkedin-ads-2.2.0.tar` & `tap-linkedin-ads-2.3.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 17:48:54.447049 tap-linkedin-ads-2.2.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-02-03 11:59:41.000000 tap-linkedin-ads-2.2.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-08 17:48:54.447049 tap-linkedin-ads-2.2.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16976 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-08 17:48:54.447049 tap-linkedin-ads-2.2.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2024-04-08 17:45:26.000000 tap-linkedin-ads-2.2.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 17:48:54.443050 tap-linkedin-ads-2.2.0/tap_linkedin_ads/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1620 2024-04-08 17:01:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14809 2024-04-08 17:39:42.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      612 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2706 2023-11-06 17:25:42.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 17:48:54.447049 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1696 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/account_users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3471 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13824 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13791 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2989 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/campaign_groups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12277 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/creatives.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/video_ads.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31980 2024-04-08 17:15:30.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5605 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12355 2023-02-03 11:59:41.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads/transform.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 17:48:54.443050 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      822 2024-04-08 17:48:54.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2024-04-08 17:48:53.000000 tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13369 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/transform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14809 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1696 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/account_users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/creatives.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13824 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5113 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/video_ads.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12277 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13791 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2989 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/campaign_groups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3471 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34765 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2706 2023-11-06 17:25:42.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/schema.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1620 2024-04-13 15:56:16.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5775 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      612 2023-02-07 16:26:29.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      814 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2024-04-15 10:01:00.000000 tap-linkedin-ads-2.3.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17019 2024-04-15 09:55:17.000000 tap-linkedin-ads-2.3.0/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tap-linkedin-ads-2.2.0/README.md` & `tap-linkedin-ads-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,19 @@
 - Replication strategy: Incremental (query all, filter results)
   - Filter: account id (from config.json)
   - Sort by: account id ascending
   - Bookmark: last_modified_time (date-time)
 - Transformations: Fields camelCase to snake_case. URNs to ids. Unix epoch millisecond integers to date-times. Audit date-times created_at and last_modified_at de-nested. String to decimal for total_budget field.
 - Children: video_ads
 
-[**video_ads**](https://docs.microsoft.com/en-us/linkedin/marketing/integrations/ads/advertising-targeting/create-and-manage-video#finders)
-- Endpoint: https://api.linkedin.com/rest/adDirectSponsoredContents
+[**video_ads**](https://learn.microsoft.com/en-us/linkedin/marketing/community-management/shares/posts-api?view=li-lms-2024-03&tabs=curl#find-posts-by-account)
+- Endpoint: https://api.linkedin.com/rest/posts
 - Primary key field: content_reference
 - Foreign keys: account_id (accounts), owner_organization_id (organizations)
+- Required scope - `r_organization_social`
 - Replication strategy: Incremental (query all, filter results)
   - Filter: account (from parent account) and owner (from parent account) (see NOTE below)
   - Bookmark: last_modified_time (date-time)
 - Transformations: Fields camelCase to snake_case. URNs to ids. Unix epoch millisecond integers to date-times. Audit date-times created_at and last_modified_at de-nested.
 - Parent: account
 **NOTE**: The parent Account **MUST** reference and **Organization** (not a Person)
 - [Campaign Manager User Roles for Video Ads](https://www.linkedin.com/help/lms/answer/90733/campaign-manager-user-roles-for-video-ads?lang=en)
```

### Comparing `tap-linkedin-ads-2.2.0/setup.py` & `tap-linkedin-ads-2.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-linkedin-ads',
-      version='2.2.0',
+      version='2.3.0',
       description='Singer.io tap for extracting data from the LinkedIn Marketing Ads API API 2.0',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_linkedin_ads'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
```

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/__init__.py` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/client.py` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from singer import metrics
 import singer
 
 LOGGER = singer.get_logger()
 BASE_URL = 'https://api.linkedin.com/rest'
 LINKEDIN_TOKEN_URI = 'https://www.linkedin.com/oauth/v2/accessToken'
 INTROSPECTION_URI = 'https://www.linkedin.com/oauth/v2/introspectToken'
-LINKEDIN_VERSION = '202304'
+LINKEDIN_VERSION = '202403'
 
 # set default timeout of 300 seconds
 REQUEST_TIMEOUT = 300
 
 class LinkedInError(Exception):
     pass
```

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/discover.py` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/discover.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schema.py` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schema.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/account_users.json` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/account_users.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/accounts.json` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/campaign_groups.json` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/campaign_groups.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/campaigns.json` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/schemas/creatives.json` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/schemas/creatives.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/streams.py` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import urllib.parse
+import re
 import copy
 import datetime
 from datetime import timedelta
 import singer
 from singer import metrics, metadata, utils
 from singer import Transformer, should_sync_field, UNIX_MILLISECONDS_INTEGER_DATETIME_PARSING
 from singer.utils import strptime_to_utc, strftime
@@ -15,16 +16,23 @@
 FIELDS_UNAVAILABLE_FOR_AD_ANALYTICS = {
     'campaign',
     'campaignId',
     'startAt',
     'endAt',
     'creative',
     'creativeId',
+    # `pivot` and `pivotValue` is not supported anymore, adding values within the code
+    'pivot',
+    'pivotValue'
 }
 
+CURSOR_BASED_PAGINATION_STREAMS = ["accounts", "campaign_groups", "campaigns", "creatives"]
+NEW_PATH_STREAMS = ["campaign_groups", "campaigns", "creatives"]
+BASE_URL = 'https://api.linkedin.com/rest'
+
 def write_bookmark(state, value, stream_name):
     """
     Write the bookmark in the state corresponding to the stream.
     """
     if 'bookmarks' not in state:
         state['bookmarks'] = {}
     state['bookmarks'][stream_name] = value
@@ -67,36 +75,47 @@
     # Loop until the last page
     while next_url:
         LOGGER.info('URL for %s: %s', stream_name, next_url)
 
         data = client.get(url=next_url, endpoint=stream_name)
         yield data
         # Fetch next page
-        next_url = get_next_url(data)
+        next_url = get_next_url(stream_name, next_url, data)
 
         LOGGER.info('%s: Synced page %s', stream_name, page)
         page = page + 1
 
-def get_next_url(data):
+def get_next_url(stream_name, next_url, data):
     """
     Prepare and return the URL to fetch the next page of records.
     """
-    next_url = None
-    links = data.get('paging', {}).get('links', [])
-    for link in links:
-        rel = link.get('rel')
-        if rel == 'next':
-            href = link.get('href')
-            if href:
-                # url must be kept encoded for the creatives endpoint.
-                # Ref - https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-creatives?view=li-lms-2023-01&tabs=http#sample-request-3
-                if "rest/creatives" in href:
-                    return 'https://api.linkedin.com{}'.format(href)
-                # Prepare next page URL
-                next_url = 'https://api.linkedin.com{}'.format(urllib.parse.unquote(href))
+    if stream_name in CURSOR_BASED_PAGINATION_STREAMS:
+        next_page_token = data.get('metadata', {}).get('nextPageToken', None)
+        if next_page_token:
+            if 'pageToken=' in next_url:
+                next_url = re.sub(r'pageToken=[^&]+', 'pageToken={}'.format(next_page_token), next_url)
+            else:
+                next_url = next_url + "&pageToken={}".format(next_page_token)
+        else:
+            next_url = None
+    else:
+        # handles index based paination
+        next_url = None
+        links = data.get('paging', {}).get('links', [])
+        for link in links:
+            rel = link.get('rel')
+            if rel == 'next':
+                href = link.get('href')
+                if href:
+                    # url must be kept encoded for the creatives endpoint.
+                    # Ref - https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-creatives?view=li-lms-2023-01&tabs=http#sample-request-3
+                    if "rest/creatives" in href:
+                        return 'https://api.linkedin.com{}'.format(href)
+                    # Prepare next page URL
+                    next_url = 'https://api.linkedin.com{}'.format(urllib.parse.unquote(href))
     return next_url
 
 def shift_sync_window(params, today, date_window_size, forced_window_size=None):
     """
     Move ahead date window by date_window_size and update params with the new date window.
     """
     current_end = datetime.date(
@@ -107,33 +126,35 @@
 
     new_end = min(today, current_end + timedelta(days=(forced_window_size if forced_window_size else date_window_size)))
 
     new_params = {**params,
                   'dateRange.start.day': current_end.day,
                   'dateRange.start.month': current_end.month,
                   'dateRange.start.year': current_end.year,
-
                   'dateRange.end.day': new_end.day,
                   'dateRange.end.month': new_end.month,
                   'dateRange.end.year': new_end.year,}
     return current_end, new_end, new_params
 
-def merge_responses(data):
+def merge_responses(pivot, data):
     """
     Prepare map with key as primary key and value as the record itself for analytics streams.
     The primary key is a combination of pivotValue and start date fields value.
     Update existing records with the same primary key value.
     """
     full_records = {}
     # Loop through each page of data
     for page in data:
         # Loop through each record of the page
         for element in page:
             temp_start = element['dateRange']['start']
-            temp_pivotValue = element['pivotValue']
+            temp_pivotValue = element['pivotValues'][0]
+            # adding pivot and pivot_value to make it compatible with the previous tap version
+            element['pivot'] = pivot
+            element["pivot_value"] = temp_pivotValue
             string_start = '{}-{}-{}'.format(temp_start['year'], temp_start['month'], temp_start['day'])
             primary_key = (temp_pivotValue, string_start)
             if primary_key in full_records:
                 # Update existing record with same primary key
                 full_records[primary_key].update(element)
             else:
                 full_records[primary_key] = element
@@ -253,24 +274,25 @@
                     else:
                         # Write record if replication key is not available in the record
                         self.write_record(transformed_record, time_extracted=time_extracted)
                         counter.increment()
 
             return max_bookmark_value, counter.value
 
-    # pylint: disable=too-many-branches,too-many-statements,too-many-arguments,too-many-locals
+    # pylint: disable=too-many-branches,too-many-statements,too-many-arguments,too-many-locals,too-many-nested-blocks
     def sync_endpoint(self,
                       client,
                       catalog,
                       state,
                       page_size,
                       start_date,
                       selected_streams,
                       date_window_size,
-                      parent_id=None):
+                      parent_id=None,
+                      account_list=None):
         """
         Sync a specific parent or child endpoint.
         """
         # Get the latest bookmark for the stream and set the last_datetime
         last_datetime = self.get_bookmark(state, start_date)
         max_bookmark_value = last_datetime
         LOGGER.info('%s: bookmark last_datetime = %s', self.tap_stream_id, max_bookmark_value)
@@ -297,157 +319,172 @@
         # Each page has a "start" (offset value) and a "count" (batch size, number of records)
         # Increase the "start" by the "count" for each batch.
         # Continue until the "start" exceeds the total_records.
         start = 0 # Starting offset value for each batch API call
         total_records = 0
         page = 1
 
-        endpoint_params = {
-            'start': start,
-            'count': page_size,
-            **self.params # adds in endpoint specific, sort, filter params
-        }
+        if self.tap_stream_id in CURSOR_BASED_PAGINATION_STREAMS:
+            # hardcoding the pagesize to 1000 for stream - accounts, as search and pageToken param can't be present at the same time.
+            if self.tap_stream_id == "accounts":
+                page_size = 1000
+            endpoint_params = {
+                'pageSize': page_size,
+                **self.params
+            }
+        else:
+            endpoint_params = {
+                'start': start,
+                'count': page_size,
+                **self.params # adds in endpoint specific, sort, filter params
+            }
 
         querystring = '&'.join(['%s=%s' % (key, value) for (key, value) in endpoint_params.items()])
-        next_url = 'https://api.linkedin.com/rest/{}?{}'.format(self.path, querystring)
 
-        while next_url: #pylint: disable=too-many-nested-blocks
-            LOGGER.info('URL for %s: %s', self.tap_stream_id, next_url)
-
-            # Get data, API request
-            data = client.get(
-                url=next_url,
-                endpoint=self.tap_stream_id,
-                headers=self.headers)
-            # time_extracted: datetime when the data was extracted from the API
-            time_extracted = utils.now()
-
-            # Transform data with transform_json from transform.py
-            #  This function converts unix datetimes, de-nests audit fields,
-            #  tranforms URNs to IDs, tranforms/abstracts variably named fields,
-            #  converts camelCase to snake_case for fieldname keys.
-            # For the Linkedin Ads API, 'elements' is always the root data_key for records.
-            # The data_key identifies the collection of records below the <root> element
-            transformed_data = [] # initialize the record list
-            if self.data_key in data:
-                transformed_data = transform_json(data, self.tap_stream_id)[self.data_key]
-            if not transformed_data or transformed_data is None:
-                LOGGER.info('No transformed_data')
-                break # No data results
-
-            pre_singer_transformed_data = copy.deepcopy(transformed_data)
-            if self.tap_stream_id in selected_streams:
-                # Process records and gets the max_bookmark_value and record_count for the set of records
-                max_bookmark_value, record_count = self.process_records(
-                    catalog=catalog,
-                    records=transformed_data,
-                    time_extracted=time_extracted,
-                    bookmark_field=bookmark_field,
-                    max_bookmark_value=max_bookmark_value,
-                    last_datetime=last_datetime,
-                    parent_id=parent_id)
-                LOGGER.info('%s, records processed: %s', self.tap_stream_id, record_count)
-                total_records = total_records + record_count
+        urllist = []
+        if self.tap_stream_id in NEW_PATH_STREAMS:
+            # As per the latest linkedin version, few url formats are modified, it expects advertiser
+            # account_id in each url path
+            for account in account_list:
+                url = "{}/adAccounts/{}/{}?{}".format(BASE_URL, account, self.path, querystring)
+                urllist.append((account, url))
+        else:
+            if self.path == 'posts':
+                url = '{}/{}?{}&dscAdAccount=urn%3Ali%3AsponsoredAccount%3A{}'.format(BASE_URL, self.path, querystring, parent_id)
+            else:
+                url = '{}/{}?{}'.format(BASE_URL, self.path, querystring)
+            urllist.append((None, url))
 
-            # Loop thru parent batch records for each children objects
-            for child_stream_name in children:
-                if child_stream_name in selected_streams:
-                    # For each parent record
-                    child_obj = STREAMS[child_stream_name]()
-
-                    for record in pre_singer_transformed_data:
-
-                        parent_id = record.get(child_obj.foreign_key)
-
-                        child_stream_params = child_obj.params
-                        # Add children filter params based on parent IDs
-                        if self.tap_stream_id == 'accounts':
-                            account = 'urn:li:sponsoredAccount:{}'.format(parent_id)
-                            owner_id = record.get('reference_organization_id', None)
-                            owner = 'urn:li:organization:{}'.format(owner_id)
-                            if child_stream_name == 'video_ads' and owner_id is not None:
-                                child_stream_params['account'] = account
-                                child_stream_params['owner'] = owner
+        for acct_id, next_url in urllist:
+            while next_url: #pylint: disable=too-many-nested-blocks
+                LOGGER.info('URL for %s: %s', self.tap_stream_id, next_url)
+
+                # Get data, API request
+                data = client.get(
+                    url=next_url,
+                    endpoint=self.tap_stream_id,
+                    headers=self.headers)
+                # time_extracted: datetime when the data was extracted from the API
+                time_extracted = utils.now()
+
+                # Transform data with transform_json from transform.py
+                #  This function converts unix datetimes, de-nests audit fields,
+                #  tranforms URNs to IDs, tranforms/abstracts variably named fields,
+                #  converts camelCase to snake_case for fieldname keys.
+                # For the Linkedin Ads API, 'elements' is always the root data_key for records.
+                # The data_key identifies the collection of records below the <root> element
+                transformed_data = [] # initialize the record list
+                if self.data_key in data:
+                    transformed_data = transform_json(data, self.tap_stream_id)[self.data_key]
+                if not transformed_data or transformed_data is None:
+                    LOGGER.info('No transformed_data')
+                    break # No data results
+
+                pre_singer_transformed_data = copy.deepcopy(transformed_data)
+                if self.tap_stream_id in selected_streams:
+                    # Process records and gets the max_bookmark_value and record_count for the set of records
+                    max_bookmark_value, record_count = self.process_records(
+                        catalog=catalog,
+                        records=transformed_data,
+                        time_extracted=time_extracted,
+                        bookmark_field=bookmark_field,
+                        max_bookmark_value=max_bookmark_value,
+                        last_datetime=last_datetime,
+                        parent_id=parent_id)
+                    LOGGER.info('%s, records processed: %s', self.tap_stream_id, record_count)
+                    total_records = total_records + record_count
+
+                # Loop thru parent batch records for each children objects
+                for child_stream_name in children:
+                    if child_stream_name in selected_streams:
+                        # For each parent record
+                        child_obj = STREAMS[child_stream_name]()
+
+                        for record in pre_singer_transformed_data:
+
+                            parent_id = record.get(child_obj.foreign_key)
+
+                            child_stream_params = child_obj.params
+                            # Add children filter params based on parent IDs
+                            if self.tap_stream_id == 'accounts':
+                                account = 'urn:li:sponsoredAccount:{}'.format(parent_id)
+                            elif self.tap_stream_id == 'campaigns':
+                                campaign = 'urn:li:sponsoredCampaign:{}'.format(parent_id)
+                                if child_stream_name == 'creatives':
+                                    # The value of the campaigns in the query params should be passed in the encoded format.
+                                    # Ref - https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-creatives?view=li-lms-2023-01&tabs=http#sample-request-3
+                                    child_stream_params['campaigns'] = 'List(urn%3Ali%3AsponsoredCampaign%3A{})'.format(parent_id)
+                                elif child_stream_name in ('ad_analytics_by_campaign', 'ad_analytics_by_creative'):
+                                    child_stream_params['campaigns[0]'] = campaign
+
+                            # Update params for the child stream
+                            child_obj.params = child_stream_params
+                            LOGGER.info('Syncing: %s, parent_stream: %s, parent_id: %s',
+                                        child_stream_name,
+                                        self.tap_stream_id,
+                                        parent_id)
+
+                            # Call sync method for the child stream
+                            if child_stream_name in {'ad_analytics_by_campaign', 'ad_analytics_by_creative'}:
+                                child_total_records, child_batch_bookmark_value = child_obj.sync_ad_analytics(
+                                    client=client,
+                                    catalog=catalog,
+                                    last_datetime=child_obj.get_bookmark(state, start_date),
+                                    date_window_size=date_window_size,
+                                    parent_id=parent_id)
                             else:
-                                LOGGER.warning("Skipping video_ads call for %s account as reference_organization_id is not found.", account)
-                                continue
-                        elif self.tap_stream_id == 'campaigns':
-                            campaign = 'urn:li:sponsoredCampaign:{}'.format(parent_id)
-                            if child_stream_name == 'creatives':
-                                # The value of the campaigns in the query params should be passed in the encoded format.
-                                # Ref - https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-creatives?view=li-lms-2023-01&tabs=http#sample-request-3
-                                child_stream_params['campaigns'] = 'List(urn%3Ali%3AsponsoredCampaign%3A{})'.format(parent_id)
-                            elif child_stream_name in ('ad_analytics_by_campaign', 'ad_analytics_by_creative'):
-                                child_stream_params['campaigns[0]'] = campaign
-
-                        # Update params for the child stream
-                        child_obj.params = child_stream_params
-                        LOGGER.info('Syncing: %s, parent_stream: %s, parent_id: %s',
-                                    child_stream_name,
-                                    self.tap_stream_id,
-                                    parent_id)
-
-                        # Call sync method for the child stream
-                        if child_stream_name in {'ad_analytics_by_campaign', 'ad_analytics_by_creative'}:
-                            child_total_records, child_batch_bookmark_value = child_obj.sync_ad_analytics(
-                                client=client,
-                                catalog=catalog,
-                                last_datetime=child_obj.get_bookmark(state, start_date),
-                                date_window_size=date_window_size,
-                                parent_id=parent_id)
-                        else:
-                            child_total_records, child_batch_bookmark_value = child_obj.sync_endpoint(
-                                client=client,
-                                catalog=catalog,
-                                state=state,
-                                page_size=page_size,
-                                start_date=start_date,
-                                selected_streams=selected_streams,
-                                date_window_size=date_window_size,
-                                parent_id=parent_id)
-
-                        child_batch_bookmark_dttm = strptime_to_utc(child_batch_bookmark_value)
-                        child_max_bookmark = child_max_bookmarks.get(child_stream_name)
-                        child_max_bookmark_dttm = strptime_to_utc(child_max_bookmark)
-                        if child_batch_bookmark_dttm > child_max_bookmark_dttm:
-                            # Update bookmark for child stream.
-                            child_max_bookmarks[child_stream_name] = strftime(child_batch_bookmark_dttm)
-
-                        LOGGER.info('Synced: %s, parent_id: %s, total_records: %s',
-                                    child_stream_name,
-                                    parent_id,
-                                    child_total_records)
-                        LOGGER.info('FINISHED Syncing: %s', child_stream_name)
-
-            # Pagination: Get next_url
-            next_url = get_next_url(data)
-
-            if self.tap_stream_id in selected_streams:
-                LOGGER.info('%s: Synced page %s, this page: %s. Total records processed: %s',
-                            self.tap_stream_id,
-                            page,
-                            record_count,
-                            total_records)
-            page = page + 1
+                                child_total_records, child_batch_bookmark_value = child_obj.sync_endpoint(
+                                    client=client,
+                                    catalog=catalog,
+                                    state=state,
+                                    page_size=page_size,
+                                    start_date=start_date,
+                                    selected_streams=selected_streams,
+                                    date_window_size=date_window_size,
+                                    parent_id=parent_id,
+                                    account_list=[acct_id])
+
+                            child_batch_bookmark_dttm = strptime_to_utc(child_batch_bookmark_value)
+                            child_max_bookmark = child_max_bookmarks.get(child_stream_name)
+                            child_max_bookmark_dttm = strptime_to_utc(child_max_bookmark)
+                            if child_batch_bookmark_dttm > child_max_bookmark_dttm:
+                                # Update bookmark for child stream.
+                                child_max_bookmarks[child_stream_name] = strftime(child_batch_bookmark_dttm)
+
+                            LOGGER.info('Synced: %s, parent_id: %s, total_records: %s',
+                                        child_stream_name,
+                                        parent_id,
+                                        child_total_records)
+                            LOGGER.info('FINISHED Syncing: %s', child_stream_name)
+
+                # Pagination: Get next_url
+                next_url = get_next_url(self.tap_stream_id, next_url, data)
+
+                if self.tap_stream_id in selected_streams:
+                    LOGGER.info('%s: Synced page %s, this page: %s. Total records processed: %s',
+                                self.tap_stream_id,
+                                page,
+                                record_count,
+                                total_records)
+                page = page + 1
 
         # Write child stream's bookmarks
         for key, val in list(child_max_bookmarks.items()):
             write_bookmark(state, val, key)
 
         return total_records, max_bookmark_value
 
     # pylint: disable=too-many-branches,too-many-statements,unused-argument
     def sync_ad_analytics(self, client, catalog, last_datetime, date_window_size, parent_id=None):
         """
         Sync method for ad_analytics_by_campaign, ad_analytics_by_creative
         """
-        # LinkedIn has a max of 20 fields per request. We cap the chunks at 17
-        # to make sure there's always room for us to append `dateRange`,
-        # `pivot`, and `pivotValue`
-        MAX_CHUNK_LENGTH = 17
+        # LinkedIn has a max of 20 fields per request. We cap the chunks at 18
+        # to make sure there's always room for us to append `dateRange`, and `pivotValues`
+        MAX_CHUNK_LENGTH = 18
 
         bookmark_field = next(iter(self.replication_keys))
 
         max_bookmark_value = last_datetime
         last_datetime_dt = strptime_to_utc(last_datetime) - timedelta(days=7)
 
         # Prepare date window for API call
@@ -476,23 +513,23 @@
         # When testing the API, if the fields in `field` all return `0` then
         # the API returns its empty response.
 
         # However, the API distinguishes between a day with non-null values
         # (even if this means the values are all `0`) and a day with null
         # values. We found that requesting these fields gives you the days with
         # non-null values
-        first_chunk = [['dateRange', 'pivot', 'pivotValue']]
+        first_chunk = [['dateRange', 'pivotValues']]
 
         chunks = first_chunk + list(split_into_chunks(valid_selected_fields, MAX_CHUNK_LENGTH))
 
         # We have to append these fields in order to ensure we get them back
         # so that we can create the composite primary key for the record and
         # to merge the multiple responses based on this primary key
         for chunk in chunks:
-            for field in ['dateRange', 'pivot', 'pivotValue']:
+            for field in ['dateRange', 'pivotValues']:
                 if field not in chunk:
                     chunk.append(field)
 
         ############### PAGINATION (for these 2 streams) ###############
         # The Tap requests LinkedIn with one Campaign ID at one time.
         # 1 Campaign permits 100 Ads
         # Considering, 1 Ad is active and the existing behavior of the tap uses 30 Day window size
@@ -509,15 +546,16 @@
                 params = {"start": 0,
                           **static_params}
                 query_string = '&'.join(['%s=%s' % (key, value) for (key, value) in params.items()])
                 LOGGER.info('Syncing %s from %s to %s', parent_id, window_start_date, window_end_date)
                 for page in sync_analytics_endpoint(client, self.tap_stream_id, self.path, query_string):
                     if page.get(self.data_key):
                         responses.append(page.get(self.data_key))
-            raw_records = merge_responses(responses)
+            pivot = params["pivot"] if "pivot" in params.keys() else None
+            raw_records = merge_responses(pivot, responses)
             time_extracted = utils.now()
 
             # While we broke the ad_analytics streams out from
             # `sync_endpoint()`, we want to process them the same. And
             # transform_json() expects a dictionary with a key equal to
             # `data_key` and its value is the response from the API
 
@@ -557,34 +595,46 @@
     replication_keys = ["last_modified_time"]
     key_properties = ["id"]
     account_filter = "search_id_values_param"
     path = "adAccounts"
     data_key = "elements"
     children = ["video_ads"]
     params = {
-        "q": "search",
-        "sort.field": "ID",
-        "sort.order": "ASCENDING"
+        "q": "search"
     }
+    headers = {'X-Restli-Protocol-Version': "2.0.0"}
 
 class VideoAds(LinkedInAds):
     """
     https://docs.microsoft.com/en-us/linkedin/marketing/integrations/ads/advertising-targeting/create-and-manage-video#finders
     """
     tap_stream_id = "video_ads"
     replication_keys = ["last_modified_time"]
     replication_method = "INCREMENTAL"
     key_properties = ["content_reference"]
     foreign_key = "id"
-    path = "adDirectSponsoredContents"
+    path = "posts"
     data_key = "elements"
     parent = "accounts"
     params = {
-        "q": "account"
+        "q": "dscAdAccount",
+        "dscAdTypes": "List(VIDEO)"
     }
+    headers = {'X-Restli-Protocol-Version': "2.0.0"}
+
+    def sync_endpoint(self, *args, **kwargs):
+        try:
+            return super().sync_endpoint(*args, **kwargs)
+        except Exception as error:
+            if "Not enough permissions to access: partnerApiPostsExternal" in str(error):
+                LOGGER.warning("Access to the video-ads API is denied due to insufficient permissions. Please reauthenticate or verify the required permissions.")
+                LOGGER.error(error)
+                # total record count (zero), initial bookmark returned to supress this failure
+                return 0, self.get_bookmark(kwargs.get("state"), kwargs.get("start_date"))
+            raise error
 
 class AccountUsers(LinkedInAds):
     """
     https://docs.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-account-users#find-ad-account-users-by-accounts
     """
     tap_stream_id = "account_users"
     replication_keys = ["last_modified_time"]
@@ -605,17 +655,15 @@
     replication_method = "INCREMENTAL"
     replication_keys = ["last_modified_time"]
     key_properties = ["id"]
     account_filter = "search_account_values_param"
     path = "adCampaignGroups"
     data_key = "elements"
     params = {
-        "q": "search",
-        "sort.field": "ID",
-        "sort.order": "ASCENDING"
+        "q": "search"
     }
 
 class Campaigns(LinkedInAds):
     """
     https://docs.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-campaigns#search-for-campaigns
     """
     tap_stream_id = "campaigns"
@@ -623,17 +671,15 @@
     replication_keys = ["last_modified_time"]
     key_properties = ["id"]
     account_filter = "search_account_values_param"
     path = "adCampaigns"
     data_key = "elements"
     children = ["ad_analytics_by_campaign", "creatives", "ad_analytics_by_creative"]
     params = {
-        "q": "search",
-        "sort.field": "ID",
-        "sort.order": "ASCENDING"
+        "q": "search"
     }
 
 class Creatives(LinkedInAds):
     """
     https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-creatives?view=li-lms-2023-01&tabs=http#search-for-creatives
     """
     tap_stream_id = "creatives"
```

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/sync.py` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,42 +101,43 @@
     for stream_name in stream_to_sync:
         stream_obj = STREAMS[stream_name]()
 
         # Add appropriate account_filter query parameters based on account_filter type
         account_filter = stream_obj.account_filter
         if config.get("accounts") and account_filter is not None:
             account_list = config['accounts'].replace(" ", "").split(",")
-            params = stream_obj.params
-            for idx, account in enumerate(account_list):
+            if len(account_list) > 0:
+                params = stream_obj.params
                 if account_filter == 'search_id_values_param':
-                    params['search.id.values[{}]'.format(idx)] = int(account)
-                elif account_filter == 'search_account_values_param':
-                    params['search.account.values[{}]'.format(idx)] = \
-                        'urn:li:sponsoredAccount:{}'.format(account)
+                    # Convert account IDs to URN format
+                    urn_list = ["urn%3Ali%3AsponsoredAccount%3A{}".format(account_id) for account_id in account_list]
+                    # Create the query parameter string
+                    param_value = "(id:(values:List({})))".format(','.join(urn_list))
+                    params['search'] = param_value
                 elif account_filter == 'accounts_param':
-                    params['accounts[{}]'.format(idx)] = \
-                        'urn:li:sponsoredAccount:{}'.format(account)
-
-            # Update params of specific stream
-            stream_obj.params = params
+                    for idx, account in enumerate(account_list):
+                        params['accounts[{}]'.format(idx)] = \
+                            'urn:li:sponsoredAccount:{}'.format(account)
+                # Update params of specific stream
+                stream_obj.params = params
 
         LOGGER.info('START Syncing: %s', stream_name)
         update_currently_syncing(state, stream_name)
 
         # Write schema for parent streams
         if stream_name in selected_streams:
             stream_obj.write_schema(catalog)
 
         total_records, max_bookmark_value = stream_obj.sync_endpoint(
             client=client, catalog=catalog,
-            state=state,
-            page_size=page_size,
+            state=state, page_size=page_size,
             start_date=start_date,
             selected_streams=selected_streams,
-            date_window_size=date_window_size)
+            date_window_size=date_window_size,
+            account_list=account_list)
 
         # Write parent stream's bookmarks
         if stream_obj.replication_keys and stream_name in selected_streams:
             write_bookmark(state, max_bookmark_value, stream_name)
 
         update_currently_syncing(state, None)
         LOGGER.info('Synced: %s, total_records: %s', stream_name, total_records)
```

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads/transform.py` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -290,28 +290,49 @@
                         # Set ID as string
                         id_val = search.group(2)
                         pass #pylint: disable=unnecessary-pass
                     data_dict[new_key] = id_val
     return data_dict
 
 
+def transform_video_ads(data_dict):
+    # pylint: disable=fixme
+    # TODO: To be removed in next major version release
+    if 'author' in data_dict:
+        data_dict['owner'] = data_dict["author"]
+    if 'id' in data_dict:
+        data_dict['content_reference'] = data_dict["id"]
+    if 'ad_context' in data_dict:
+        if 'dsc_name' in data_dict['ad_context']:
+            data_dict['name'] = data_dict["ad_context"]['dsc_name']
+        if 'dsc_ad_type' in data_dict['ad_context']:
+            data_dict['type'] = data_dict["ad_context"]['dsc_ad_type']
+        if 'dsc_ad_account' in data_dict['ad_context']:
+            data_dict['account'] = data_dict["ad_context"]['dsc_ad_account']
+    if 'last_modified_at' in data_dict:
+        data_dict['last_modified_time'] = data_dict["last_modified_at"]
+    if 'created_at' in data_dict:
+        data_dict['created_time'] = data_dict["created_at"]
+    return data_dict
 
 def transform_data(data_dict, stream_name):
     new_dict = data_dict
     i = 0
     for record in data_dict['elements']:
         this_dict = record
         if stream_name.startswith('ad_analytics_by_'):
             this_dict = transform_analytics(this_dict)
         elif stream_name == 'accounts':
             this_dict = transform_accounts(this_dict)
         elif stream_name == 'campaigns':
             this_dict = transform_campaigns(this_dict)
         elif stream_name == 'creatives':
             this_dict = transform_creatives(this_dict)
+        elif stream_name == 'video_ads':
+            this_dict = transform_video_ads(this_dict)
         this_dict = transform_urn(this_dict)
         this_dict = transform_audit_fields(this_dict)
 
         new_dict['elements'][i] = this_dict
         i = i + 1
     return new_dict
```

### Comparing `tap-linkedin-ads-2.2.0/tap_linkedin_ads.egg-info/SOURCES.txt` & `tap-linkedin-ads-2.3.0/tap_linkedin_ads.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 tap_linkedin_ads/__init__.py
 tap_linkedin_ads/client.py
 tap_linkedin_ads/discover.py
 tap_linkedin_ads/schema.py
 tap_linkedin_ads/streams.py
```

