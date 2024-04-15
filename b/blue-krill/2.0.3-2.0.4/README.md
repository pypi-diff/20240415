# Comparing `tmp/blue_krill-2.0.3.tar.gz` & `tmp/blue_krill-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_krill-2.0.3.tar", max compression
+gzip compressed data, was "blue_krill-2.0.4.tar", max compression
```

## Comparing `blue_krill-2.0.3.tar` & `blue_krill-2.0.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    23869 2024-04-07 07:29:59.357875 blue_krill-2.0.3/README.md
--rw-r--r--   0        0        0      782 2024-04-07 07:32:22.155885 blue_krill-2.0.3/blue_krill/__init__.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/async_utils/__init__.py
--rw-r--r--   0        0        0     1755 2023-06-29 08:21:26.533385 blue_krill-2.0.3/blue_krill/async_utils/django_utils.py
--rw-r--r--   0        0        0    11538 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/async_utils/poll_task.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/auth/__init__.py
--rw-r--r--   0        0        0     6068 2022-05-18 02:32:27.384264 blue_krill-2.0.3/blue_krill/auth/client.py
--rw-r--r--   0        0        0     2683 2023-12-08 11:06:39.820998 blue_krill-2.0.3/blue_krill/auth/jwt.py
--rw-r--r--   0        0        0     1629 2023-12-08 11:21:15.853208 blue_krill-2.0.3/blue_krill/auth/utils.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/connections/__init__.py
--rw-r--r--   0        0        0      824 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/connections/exceptions.py
--rw-r--r--   0        0        0     1718 2022-07-05 03:48:54.805230 blue_krill-2.0.3/blue_krill/connections/ha_algorithm.py
--rw-r--r--   0        0        0     7147 2022-07-05 03:48:54.805230 blue_krill-2.0.3/blue_krill/connections/ha_endpoint_pool.py
--rw-r--r--   0        0        0     1457 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/contextlib.py
--rw-r--r--   0        0        0     6964 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/cubing_case.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/data_types/__init__.py
--rw-r--r--   0        0        0     8652 2022-05-11 07:34:37.799061 blue_krill-2.0.3/blue_krill/data_types/enum.py
--rw-r--r--   0        0        0     3603 2023-12-08 11:05:35.944110 blue_krill-2.0.3/blue_krill/data_types/url.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/editions/__init__.py
--rw-r--r--   0        0        0    21435 2024-04-07 07:29:59.357875 blue_krill-2.0.3/blue_krill/editions/editionctl.py
--rw-r--r--   0        0        0     2777 2023-12-08 11:20:10.900303 blue_krill-2.0.3/blue_krill/encoding.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/encrypt/__init__.py
--rw-r--r--   0        0        0     4419 2024-04-07 07:29:59.357875 blue_krill-2.0.3/blue_krill/encrypt/handler.py
--rw-r--r--   0        0        0     2399 2022-05-11 07:34:37.799061 blue_krill-2.0.3/blue_krill/encrypt/legacy.py
--rw-r--r--   0        0        0     1980 2023-08-16 01:47:28.698321 blue_krill-2.0.3/blue_krill/encrypt/utils.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/models/__init__.py
--rw-r--r--   0        0        0      867 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/models/better_loaddata/__init__.py
--rw-r--r--   0        0        0      882 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/models/better_loaddata/apps.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/models/better_loaddata/management/__init__.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/models/better_loaddata/management/commands/__init__.py
--rw-r--r--   0        0        0     5277 2024-04-07 07:29:59.357875 blue_krill-2.0.3/blue_krill/models/better_loaddata/management/commands/better_loaddata.py
--rw-r--r--   0        0        0     1727 2023-08-16 01:47:28.698321 blue_krill-2.0.3/blue_krill/models/fields.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/monitoring/__init__.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/monitoring/probe/__init__.py
--rw-r--r--   0        0        0     3827 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/monitoring/probe/base.py
--rw-r--r--   0        0        0      906 2022-05-11 07:34:37.799061 blue_krill-2.0.3/blue_krill/monitoring/probe/exceptions.py
--rw-r--r--   0        0        0     3723 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/monitoring/probe/http.py
--rw-r--r--   0        0        0     2689 2024-04-07 07:29:59.357875 blue_krill-2.0.3/blue_krill/monitoring/probe/mysql.py
--rw-r--r--   0        0        0     2906 2023-06-29 08:21:26.533385 blue_krill-2.0.3/blue_krill/monitoring/probe/redis.py
--rw-r--r--   0        0        0     1908 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/monitoring/probe/tcp.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/monitoring/prometheus/__init__.py
--rw-r--r--   0        0        0     5004 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/monitoring/prometheus/django_utils.py
--rw-r--r--   0        0        0     1344 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/monitoring/prometheus/setups.py
--rw-r--r--   0        0        0        0 2022-05-11 07:34:37.799061 blue_krill-2.0.3/blue_krill/py.typed
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/redis_tools/__init__.py
--rw-r--r--   0        0        0     6517 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/redis_tools/messaging.py
--rw-r--r--   0        0        0     3756 2023-08-16 01:47:28.698321 blue_krill-2.0.3/blue_krill/redis_tools/sentinel.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/secure/__init__.py
--rw-r--r--   0        0        0     3886 2022-05-11 07:34:37.799061 blue_krill-2.0.3/blue_krill/secure/bk_secure.py
--rw-r--r--   0        0        0     2233 2022-05-11 07:34:37.799061 blue_krill-2.0.3/blue_krill/secure/dj_environ.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/storages/__init__.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/storages/blobstore/__init__.py
--rw-r--r--   0        0        0     4045 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/storages/blobstore/base.py
--rw-r--r--   0        0        0    13906 2023-06-29 08:21:26.533385 blue_krill-2.0.3/blue_krill/storages/blobstore/bkrepo.py
--rw-r--r--   0        0        0     1910 2022-06-30 02:37:39.021448 blue_krill-2.0.3/blue_krill/storages/blobstore/exceptions.py
--rw-r--r--   0        0        0     6262 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/storages/blobstore/s3.py
--rw-r--r--   0        0        0    10889 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/termcolors.py
--rw-r--r--   0        0        0     1666 2023-12-08 11:08:45.350747 blue_krill-2.0.3/blue_krill/text.py
--rw-r--r--   0        0        0      760 2022-04-25 06:52:48.581028 blue_krill-2.0.3/blue_krill/web/__init__.py
--rw-r--r--   0        0        0     9697 2022-05-11 07:34:37.799061 blue_krill-2.0.3/blue_krill/web/drf_utils.py
--rw-r--r--   0        0        0     5644 2022-05-18 02:32:27.384264 blue_krill-2.0.3/blue_krill/web/std_error.py
--rw-r--r--   0        0        0     2273 2024-04-07 07:32:25.735936 blue_krill-2.0.3/pyproject.toml
--rw-r--r--   0        0        0    24876 1970-01-01 00:00:00.000000 blue_krill-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    23869 2023-12-28 08:29:17.388998 blue_krill-2.0.4/README.md
+-rw-r--r--   0        0        0      782 2024-04-12 02:27:23.381778 blue_krill-2.0.4/blue_krill/__init__.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.390141 blue_krill-2.0.4/blue_krill/async_utils/__init__.py
+-rw-r--r--   0        0        0     1755 2023-12-28 08:29:17.390576 blue_krill-2.0.4/blue_krill/async_utils/django_utils.py
+-rw-r--r--   0        0        0    11538 2023-12-28 08:29:17.390955 blue_krill-2.0.4/blue_krill/async_utils/poll_task.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.391519 blue_krill-2.0.4/blue_krill/auth/__init__.py
+-rw-r--r--   0        0        0     6068 2023-12-28 08:29:17.392007 blue_krill-2.0.4/blue_krill/auth/client.py
+-rw-r--r--   0        0        0     2683 2023-12-28 08:29:17.392392 blue_krill-2.0.4/blue_krill/auth/jwt.py
+-rw-r--r--   0        0        0     1629 2023-12-28 08:29:17.392726 blue_krill-2.0.4/blue_krill/auth/utils.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.393231 blue_krill-2.0.4/blue_krill/connections/__init__.py
+-rw-r--r--   0        0        0      824 2023-12-28 08:29:17.393674 blue_krill-2.0.4/blue_krill/connections/exceptions.py
+-rw-r--r--   0        0        0     1718 2023-12-28 08:29:17.394090 blue_krill-2.0.4/blue_krill/connections/ha_algorithm.py
+-rw-r--r--   0        0        0     7147 2023-12-28 08:29:17.394652 blue_krill-2.0.4/blue_krill/connections/ha_endpoint_pool.py
+-rw-r--r--   0        0        0     1457 2023-12-28 08:29:17.395008 blue_krill-2.0.4/blue_krill/contextlib.py
+-rw-r--r--   0        0        0     6964 2023-12-28 08:29:17.395447 blue_krill-2.0.4/blue_krill/cubing_case.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.395972 blue_krill-2.0.4/blue_krill/data_types/__init__.py
+-rw-r--r--   0        0        0     8652 2023-12-28 08:29:17.396562 blue_krill-2.0.4/blue_krill/data_types/enum.py
+-rw-r--r--   0        0        0     3603 2023-12-28 08:29:17.396943 blue_krill-2.0.4/blue_krill/data_types/url.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.397595 blue_krill-2.0.4/blue_krill/editions/__init__.py
+-rw-r--r--   0        0        0    21435 2023-12-28 08:29:17.398764 blue_krill-2.0.4/blue_krill/editions/editionctl.py
+-rw-r--r--   0        0        0     2777 2023-12-28 08:29:17.399375 blue_krill-2.0.4/blue_krill/encoding.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.399996 blue_krill-2.0.4/blue_krill/encrypt/__init__.py
+-rw-r--r--   0        0        0     4419 2023-12-28 08:29:17.400628 blue_krill-2.0.4/blue_krill/encrypt/handler.py
+-rw-r--r--   0        0        0     2399 2023-12-28 08:29:17.402300 blue_krill-2.0.4/blue_krill/encrypt/legacy.py
+-rw-r--r--   0        0        0     1894 2024-04-12 02:27:23.382245 blue_krill-2.0.4/blue_krill/encrypt/utils.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.403663 blue_krill-2.0.4/blue_krill/models/__init__.py
+-rw-r--r--   0        0        0      867 2023-12-28 08:29:17.405271 blue_krill-2.0.4/blue_krill/models/better_loaddata/__init__.py
+-rw-r--r--   0        0        0      882 2023-12-28 08:29:17.406240 blue_krill-2.0.4/blue_krill/models/better_loaddata/apps.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.407079 blue_krill-2.0.4/blue_krill/models/better_loaddata/management/__init__.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.408623 blue_krill-2.0.4/blue_krill/models/better_loaddata/management/commands/__init__.py
+-rw-r--r--   0        0        0     5277 2024-04-09 02:56:24.296363 blue_krill-2.0.4/blue_krill/models/better_loaddata/management/commands/better_loaddata.py
+-rw-r--r--   0        0        0     1727 2023-12-28 08:29:17.410438 blue_krill-2.0.4/blue_krill/models/fields.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.410983 blue_krill-2.0.4/blue_krill/monitoring/__init__.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.411485 blue_krill-2.0.4/blue_krill/monitoring/probe/__init__.py
+-rw-r--r--   0        0        0     3827 2023-12-28 08:29:17.411818 blue_krill-2.0.4/blue_krill/monitoring/probe/base.py
+-rw-r--r--   0        0        0      906 2023-12-28 08:29:17.412141 blue_krill-2.0.4/blue_krill/monitoring/probe/exceptions.py
+-rw-r--r--   0        0        0     3723 2023-12-28 08:29:17.412464 blue_krill-2.0.4/blue_krill/monitoring/probe/http.py
+-rw-r--r--   0        0        0     2689 2023-12-28 08:29:17.412802 blue_krill-2.0.4/blue_krill/monitoring/probe/mysql.py
+-rw-r--r--   0        0        0     2906 2023-12-28 08:29:17.413153 blue_krill-2.0.4/blue_krill/monitoring/probe/redis.py
+-rw-r--r--   0        0        0     1908 2023-12-28 08:29:17.413536 blue_krill-2.0.4/blue_krill/monitoring/probe/tcp.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.414048 blue_krill-2.0.4/blue_krill/monitoring/prometheus/__init__.py
+-rw-r--r--   0        0        0     5004 2023-12-28 08:29:17.414466 blue_krill-2.0.4/blue_krill/monitoring/prometheus/django_utils.py
+-rw-r--r--   0        0        0     1344 2023-12-28 08:29:17.414790 blue_krill-2.0.4/blue_krill/monitoring/prometheus/setups.py
+-rw-r--r--   0        0        0        0 2023-12-28 08:29:17.414918 blue_krill-2.0.4/blue_krill/py.typed
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.415552 blue_krill-2.0.4/blue_krill/redis_tools/__init__.py
+-rw-r--r--   0        0        0     6517 2023-12-28 08:29:17.415985 blue_krill-2.0.4/blue_krill/redis_tools/messaging.py
+-rw-r--r--   0        0        0     3756 2023-12-28 08:29:17.416377 blue_krill-2.0.4/blue_krill/redis_tools/sentinel.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.417023 blue_krill-2.0.4/blue_krill/secure/__init__.py
+-rw-r--r--   0        0        0     3886 2023-12-28 08:29:17.417580 blue_krill-2.0.4/blue_krill/secure/bk_secure.py
+-rw-r--r--   0        0        0     2233 2023-12-28 08:29:17.418108 blue_krill-2.0.4/blue_krill/secure/dj_environ.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.418641 blue_krill-2.0.4/blue_krill/storages/__init__.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.419158 blue_krill-2.0.4/blue_krill/storages/blobstore/__init__.py
+-rw-r--r--   0        0        0     4045 2023-12-28 08:29:17.419667 blue_krill-2.0.4/blue_krill/storages/blobstore/base.py
+-rw-r--r--   0        0        0    13906 2023-12-28 08:29:17.420197 blue_krill-2.0.4/blue_krill/storages/blobstore/bkrepo.py
+-rw-r--r--   0        0        0     1910 2023-12-28 08:29:17.420553 blue_krill-2.0.4/blue_krill/storages/blobstore/exceptions.py
+-rw-r--r--   0        0        0     6262 2023-12-28 08:29:17.420985 blue_krill-2.0.4/blue_krill/storages/blobstore/s3.py
+-rw-r--r--   0        0        0    10889 2023-12-28 08:29:17.421400 blue_krill-2.0.4/blue_krill/termcolors.py
+-rw-r--r--   0        0        0     1666 2023-12-28 08:29:17.421739 blue_krill-2.0.4/blue_krill/text.py
+-rw-r--r--   0        0        0      760 2023-12-28 08:29:17.422249 blue_krill-2.0.4/blue_krill/web/__init__.py
+-rw-r--r--   0        0        0     9697 2023-12-28 08:29:17.422694 blue_krill-2.0.4/blue_krill/web/drf_utils.py
+-rw-r--r--   0        0        0     5644 2023-12-28 08:29:17.423132 blue_krill-2.0.4/blue_krill/web/std_error.py
+-rw-r--r--   0        0        0     2273 2024-04-12 02:27:23.382788 blue_krill-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0    24876 1970-01-01 00:00:00.000000 blue_krill-2.0.4/PKG-INFO
```

### Comparing `blue_krill-2.0.3/README.md` & `blue_krill-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/__init__.py` & `blue_krill-2.0.4/blue_krill/models/better_loaddata/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,8 +4,9 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-__version__ = "2.0.3"
+# -*- coding: utf-8 -*-
+default_app_config = 'blue_krill.models.better_loaddata.apps.BetterLoadDataConfig'
```

### Comparing `blue_krill-2.0.3/blue_krill/async_utils/__init__.py` & `blue_krill-2.0.4/blue_krill/async_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/async_utils/django_utils.py` & `blue_krill-2.0.4/blue_krill/async_utils/django_utils.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/async_utils/poll_task.py` & `blue_krill-2.0.4/blue_krill/async_utils/poll_task.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/auth/__init__.py` & `blue_krill-2.0.4/blue_krill/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/auth/client.py` & `blue_krill-2.0.4/blue_krill/auth/client.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/auth/jwt.py` & `blue_krill-2.0.4/blue_krill/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/auth/utils.py` & `blue_krill-2.0.4/blue_krill/auth/utils.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/connections/__init__.py` & `blue_krill-2.0.4/blue_krill/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/connections/exceptions.py` & `blue_krill-2.0.4/blue_krill/connections/exceptions.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/connections/ha_algorithm.py` & `blue_krill-2.0.4/blue_krill/connections/ha_algorithm.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/connections/ha_endpoint_pool.py` & `blue_krill-2.0.4/blue_krill/connections/ha_endpoint_pool.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/contextlib.py` & `blue_krill-2.0.4/blue_krill/contextlib.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/cubing_case.py` & `blue_krill-2.0.4/blue_krill/cubing_case.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/data_types/__init__.py` & `blue_krill-2.0.4/blue_krill/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/data_types/enum.py` & `blue_krill-2.0.4/blue_krill/data_types/enum.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/data_types/url.py` & `blue_krill-2.0.4/blue_krill/data_types/url.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/editions/__init__.py` & `blue_krill-2.0.4/blue_krill/editions/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/editions/editionctl.py` & `blue_krill-2.0.4/blue_krill/editions/editionctl.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/encoding.py` & `blue_krill-2.0.4/blue_krill/encoding.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/encrypt/__init__.py` & `blue_krill-2.0.4/blue_krill/encrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/encrypt/handler.py` & `blue_krill-2.0.4/blue_krill/encrypt/handler.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/encrypt/legacy.py` & `blue_krill-2.0.4/blue_krill/encrypt/legacy.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/encrypt/utils.py` & `blue_krill-2.0.4/blue_krill/encrypt/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,28 +20,25 @@
 
 def get_default_secret_key():
     try:
         from django.conf import settings
 
         return settings.BKKRILL_ENCRYPT_SECRET_KEY
     except ImportError:
-        logger.exception("you should supply a default secret key")
-        raise
+        return None
 
 
 def get_default_encrypt_cipher_type():
     """获取默认的加密算法"""
-
     try:
         from django.conf import settings
 
-        return settings.ENCRYPT_CIPHER_TYPE
+        return getattr(settings, 'ENCRYPT_CIPHER_TYPE', 'FernetCipher')
     except ImportError:
-        logger.exception("you should supply a encrypt cipher type")
-        raise
+        return 'FernetCipher'
 
 
 def encrypt_string(s: str, key: Optional[bytes] = None) -> str:
     """Shortcut function: encrypt a string into a fernet token"""
     key = key or get_default_secret_key()
     f = Fernet(key)
     value = f.encrypt(force_bytes(s))
```

### Comparing `blue_krill-2.0.3/blue_krill/models/__init__.py` & `blue_krill-2.0.4/blue_krill/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/models/better_loaddata/__init__.py` & `blue_krill-2.0.4/blue_krill/models/better_loaddata/apps.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,9 +4,12 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-# -*- coding: utf-8 -*-
-default_app_config = 'blue_krill.models.better_loaddata.apps.BetterLoadDataConfig'
+from django.apps import AppConfig
+
+
+class BetterLoadDataConfig(AppConfig):
+    name = "blue_krill.models.better_loaddata"
```

### Comparing `blue_krill-2.0.3/blue_krill/models/better_loaddata/apps.py` & `blue_krill-2.0.4/blue_krill/monitoring/probe/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,12 +4,12 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-from django.apps import AppConfig
 
 
-class BetterLoadDataConfig(AppConfig):
-    name = "blue_krill.models.better_loaddata"
+class NoFatalIssueError(Exception):
+    def __init__(self, *args, **kwargs):
+        super().__init__("no exact fatal issue, please offer one")
```

### Comparing `blue_krill-2.0.3/blue_krill/models/better_loaddata/management/__init__.py` & `blue_krill-2.0.4/blue_krill/models/better_loaddata/management/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/models/better_loaddata/management/commands/__init__.py` & `blue_krill-2.0.4/blue_krill/models/better_loaddata/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/models/better_loaddata/management/commands/better_loaddata.py` & `blue_krill-2.0.4/blue_krill/models/better_loaddata/management/commands/better_loaddata.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/models/fields.py` & `blue_krill-2.0.4/blue_krill/models/fields.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/__init__.py` & `blue_krill-2.0.4/blue_krill/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/probe/__init__.py` & `blue_krill-2.0.4/blue_krill/monitoring/probe/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/probe/base.py` & `blue_krill-2.0.4/blue_krill/monitoring/probe/base.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/probe/exceptions.py` & `blue_krill-2.0.4/blue_krill/monitoring/prometheus/setups.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,12 +4,26 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
+import os
 
+MULTIPROC_ENV_NAME = 'prometheus_multiproc_dir'
+DEFAULT_DATA_PATH = '_prometheus_data'
 
-class NoFatalIssueError(Exception):
-    def __init__(self, *args, **kwargs):
-        super().__init__("no exact fatal issue, please offer one")
+
+def setup_multiproc_dir(data_path: str = DEFAULT_DATA_PATH):
+    """Setup multi processes directory
+
+    :param data_path: if MULTIPROC_ENV_NAME has already been configured in env vars, then the
+        data_path parameter won't be used at all
+    """
+    dirname = os.environ.setdefault(MULTIPROC_ENV_NAME, data_path)
+    try:
+        os.mkdir(dirname)
+    except FileExistsError:
+        pass
+    except IOError as e:
+        print(f'unable to make prometheus data directory: {e}')
```

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/probe/http.py` & `blue_krill-2.0.4/blue_krill/monitoring/probe/http.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/probe/mysql.py` & `blue_krill-2.0.4/blue_krill/monitoring/probe/mysql.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/probe/redis.py` & `blue_krill-2.0.4/blue_krill/monitoring/probe/redis.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/probe/tcp.py` & `blue_krill-2.0.4/blue_krill/monitoring/probe/tcp.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/prometheus/__init__.py` & `blue_krill-2.0.4/blue_krill/monitoring/prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/prometheus/django_utils.py` & `blue_krill-2.0.4/blue_krill/monitoring/prometheus/django_utils.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/monitoring/prometheus/setups.py` & `blue_krill-2.0.4/blue_krill/text.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,26 +4,37 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-import os
+import sys
 
-MULTIPROC_ENV_NAME = 'prometheus_multiproc_dir'
-DEFAULT_DATA_PATH = '_prometheus_data'
+from blue_krill.data_types.url import MutableURL
 
 
-def setup_multiproc_dir(data_path: str = DEFAULT_DATA_PATH):
-    """Setup multi processes directory
+def remove_suffix(s: str, suffix: str) -> str:
+    """If given string endswith `suffix`, remove the suffix and return the new string"""
+    if sys.version_info >= (3, 9):
+        return s.removesuffix(suffix)
+    if s.endswith(suffix):
+        return s[: -len(suffix)]
+    return s
 
-    :param data_path: if MULTIPROC_ENV_NAME has already been configured in env vars, then the
-        data_path parameter won't be used at all
+
+def remove_prefix(s: str, prefix: str) -> str:
+    """If given string startswith `prefix`, remove the prefix and return the new string"""
+    if sys.version_info >= (3, 9):
+        return s.removeprefix(prefix)
+    if s.startswith(prefix):
+        return s[len(prefix) :]
+    return s
+
+
+def desensitize_url(url: str) -> str:
+    """Obscure the password field in the url
+
+    >>> desensitize_url("scheme://username:password@hostname:6666/path/?foo=bar")
+    "scheme://username:********@hostname:6666/path/?foo=bar"
     """
-    dirname = os.environ.setdefault(MULTIPROC_ENV_NAME, data_path)
-    try:
-        os.mkdir(dirname)
-    except FileExistsError:
-        pass
-    except IOError as e:
-        print(f'unable to make prometheus data directory: {e}')
+    return MutableURL(url).obscure()
```

### Comparing `blue_krill-2.0.3/blue_krill/redis_tools/__init__.py` & `blue_krill-2.0.4/blue_krill/redis_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/redis_tools/messaging.py` & `blue_krill-2.0.4/blue_krill/redis_tools/messaging.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/redis_tools/sentinel.py` & `blue_krill-2.0.4/blue_krill/redis_tools/sentinel.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/secure/__init__.py` & `blue_krill-2.0.4/blue_krill/secure/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/secure/bk_secure.py` & `blue_krill-2.0.4/blue_krill/secure/bk_secure.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/secure/dj_environ.py` & `blue_krill-2.0.4/blue_krill/secure/dj_environ.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/storages/__init__.py` & `blue_krill-2.0.4/blue_krill/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/storages/blobstore/__init__.py` & `blue_krill-2.0.4/blue_krill/storages/blobstore/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/storages/blobstore/base.py` & `blue_krill-2.0.4/blue_krill/storages/blobstore/base.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/storages/blobstore/bkrepo.py` & `blue_krill-2.0.4/blue_krill/storages/blobstore/bkrepo.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/storages/blobstore/exceptions.py` & `blue_krill-2.0.4/blue_krill/storages/blobstore/exceptions.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/storages/blobstore/s3.py` & `blue_krill-2.0.4/blue_krill/storages/blobstore/s3.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/termcolors.py` & `blue_krill-2.0.4/blue_krill/termcolors.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/web/__init__.py` & `blue_krill-2.0.4/blue_krill/web/__init__.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/web/drf_utils.py` & `blue_krill-2.0.4/blue_krill/web/drf_utils.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/blue_krill/web/std_error.py` & `blue_krill-2.0.4/blue_krill/web/std_error.py`

 * *Files identical despite different names*

### Comparing `blue_krill-2.0.3/pyproject.toml` & `blue_krill-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blue-krill"
-version = "2.0.3"
+version = "2.0.4"
 description = "Tools and common packages for blueking PaaS platform."
 include = ["blue_krill/py.typed"]
 readme = "README.md"
 authors = ["blueking <blueking@tencent.com>"]
 license = "MIT"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `blue_krill-2.0.3/PKG-INFO` & `blue_krill-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue-krill
-Version: 2.0.3
+Version: 2.0.4
 Summary: Tools and common packages for blueking PaaS platform.
 License: MIT
 Author: blueking
 Author-email: blueking@tencent.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

