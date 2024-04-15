# Comparing `tmp/alibabacloud_dingtalk-2.0.94.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.94.tar", last modified: Tue Apr  9 03:07:04 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.95.tar", last modified: Mon Apr 15 10:46:03 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.94.tar` & `alibabacloud_dingtalk-2.0.95.tar`

### file list

```diff
@@ -1,425 +1,429 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/
--rw-r--r--   0 root         (0) root         (0)   118791 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2565 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2650 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15045 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17118 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18818 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38246 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    50325 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22974 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   168107 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45004 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26721 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95304 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   142688 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204138 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   393347 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60886 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5222 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4059 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250270 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   651992 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71584 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101499 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9792 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161860 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   394680 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41039 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78198 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   236838 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119949 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143706 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   201494 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   122524 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   334068 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   418722 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41482 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33392 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44364 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30172 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19630 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8944 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14272 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5652 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10226 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   252718 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   604351 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45878 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499475 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148230 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54091 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64765 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    80337 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259804 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   315211 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   213190 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379351 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19496 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   190495 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   557050 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   850115 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113146 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120009 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18589 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   378556 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   527163 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161906 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   305557 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17280 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28173 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35856 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52698 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4825 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4965 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   134962 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18223 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68862 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119612 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136761 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   208587 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   303006 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   368637 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24693 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33051 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89450 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   671658 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   913856 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152590 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105975 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   131540 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5150 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4229 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22736 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   170469 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52481 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25614 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31620 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34360 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42471 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7167 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89094 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   161460 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120360 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57967 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68049 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   265120 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   409387 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43482 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169147 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   103368 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93324 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   146182 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44633 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   386598 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   538012 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94517 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346388 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58076 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94327 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28049 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70520 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152094 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15723 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21167 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17009 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73122 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129616 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   107789 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33103 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40753 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20146 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   128063 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8155 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41320 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42730 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194138 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   407479 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   488736 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   727920 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14081 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/
+-rw-r--r--   0 root         (0) root         (0)   120327 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15045 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17118 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18818 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38246 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    50325 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22974 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   168107 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12444 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    19284 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45004 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26721 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95304 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   142688 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204138 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   393347 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60886 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250270 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   651992 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71584 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101499 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161860 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   394680 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41039 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78198 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   236838 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119949 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143706 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   201494 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   122524 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334068 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   418722 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41482 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33392 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44364 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30172 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19630 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8944 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14272 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   257462 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   615355 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7215 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45878 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499475 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148230 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54091 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64765 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    80337 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259804 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   315211 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   213190 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379351 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19496 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   190495 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   557050 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   850115 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113146 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120009 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18589 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   378556 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   527163 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161906 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   305557 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17280 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28173 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35856 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52698 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   134962 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18223 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68862 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119612 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136761 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   208587 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   303006 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   368637 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24693 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33051 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89450 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   671658 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   913856 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152590 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105975 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   131540 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22736 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   170469 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52481 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25614 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31620 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34360 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42471 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7167 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89094 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   161460 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120360 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57967 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68049 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   265120 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   409387 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43482 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169147 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   103368 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93324 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   146182 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44633 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   386598 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   538012 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94517 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346388 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58076 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94327 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28049 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70520 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152094 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15723 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21167 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17009 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77172 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133813 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   107789 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33103 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40753 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20146 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   128063 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8155 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41320 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42730 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198336 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413640 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494302 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   740928 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14206 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-15 10:46:03.000000 alibabacloud_dingtalk-2.0.95/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.94/ChangeLog.md` & `alibabacloud_dingtalk-2.0.95/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-09 Version: 2.0.94
+- Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-04-02 Version: 2.0.93
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-03-26 Version: 2.0.92
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-03-21 Version: 2.0.91
```

### Comparing `alibabacloud_dingtalk-2.0.94/LICENSE` & `alibabacloud_dingtalk-2.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/PKG-INFO` & `alibabacloud_dingtalk-2.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.94
+Version: 2.0.95
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.94/README-CN.md` & `alibabacloud_dingtalk-2.0.95/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/README.md` & `alibabacloud_dingtalk-2.0.95/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2459,14 +2459,112 @@
         self,
         request: dingtalkcrm__1__0_models.DescribeRelationMetaRequest,
     ) -> dingtalkcrm__1__0_models.DescribeRelationMetaResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkcrm__1__0_models.DescribeRelationMetaHeaders()
         return await self.describe_relation_meta_with_options_async(request, headers, runtime)
 
+    def find_target_related_follow_records_with_options(
+        self,
+        request: dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsRequest,
+        headers: dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.follow_target_data_id):
+            body['followTargetDataId'] = request.follow_target_data_id
+        if not UtilClient.is_unset(request.follow_target_type):
+            body['followTargetType'] = request.follow_target_type
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='FindTargetRelatedFollowRecords',
+            version='crm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/crm/targetFollowRecords/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def find_target_related_follow_records_with_options_async(
+        self,
+        request: dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsRequest,
+        headers: dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.follow_target_data_id):
+            body['followTargetDataId'] = request.follow_target_data_id
+        if not UtilClient.is_unset(request.follow_target_type):
+            body['followTargetType'] = request.follow_target_type
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='FindTargetRelatedFollowRecords',
+            version='crm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/crm/targetFollowRecords/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def find_target_related_follow_records(
+        self,
+        request: dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsRequest,
+    ) -> dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsHeaders()
+        return self.find_target_related_follow_records_with_options(request, headers, runtime)
+
+    async def find_target_related_follow_records_async(
+        self,
+        request: dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsRequest,
+    ) -> dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcrm__1__0_models.FindTargetRelatedFollowRecordsHeaders()
+        return await self.find_target_related_follow_records_with_options_async(request, headers, runtime)
+
     def get_all_customer_recycles_with_options(
         self,
         request: dingtalkcrm__1__0_models.GetAllCustomerRecyclesRequest,
         headers: dingtalkcrm__1__0_models.GetAllCustomerRecyclesHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcrm__1__0_models.GetAllCustomerRecyclesResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9753,14 +9753,331 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRelationMetaResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class FindTargetRelatedFollowRecordsHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class FindTargetRelatedFollowRecordsRequest(TeaModel):
+    def __init__(
+        self,
+        follow_target_data_id: str = None,
+        follow_target_type: str = None,
+        max_results: int = None,
+        next_token: str = None,
+    ):
+        self.follow_target_data_id = follow_target_data_id
+        self.follow_target_type = follow_target_type
+        self.max_results = max_results
+        self.next_token = next_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.follow_target_data_id is not None:
+            result['followTargetDataId'] = self.follow_target_data_id
+        if self.follow_target_type is not None:
+            result['followTargetType'] = self.follow_target_type
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('followTargetDataId') is not None:
+            self.follow_target_data_id = m.get('followTargetDataId')
+        if m.get('followTargetType') is not None:
+            self.follow_target_type = m.get('followTargetType')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        return self
+
+
+class FindTargetRelatedFollowRecordsResponseBodyResultResultListFollowContent(TeaModel):
+    def __init__(
+        self,
+        biz_alias: str = None,
+        extend_value: str = None,
+        key: str = None,
+        value: str = None,
+    ):
+        self.biz_alias = biz_alias
+        self.extend_value = extend_value
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_alias is not None:
+            result['bizAlias'] = self.biz_alias
+        if self.extend_value is not None:
+            result['extendValue'] = self.extend_value
+        if self.key is not None:
+            result['key'] = self.key
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('bizAlias') is not None:
+            self.biz_alias = m.get('bizAlias')
+        if m.get('extendValue') is not None:
+            self.extend_value = m.get('extendValue')
+        if m.get('key') is not None:
+            self.key = m.get('key')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
+class FindTargetRelatedFollowRecordsResponseBodyResultResultList(TeaModel):
+    def __init__(
+        self,
+        creator_user_id: str = None,
+        follow_content: List[FindTargetRelatedFollowRecordsResponseBodyResultResultListFollowContent] = None,
+        follow_target_data_id: str = None,
+        follow_target_type: str = None,
+        gmt_create_milliseconds: str = None,
+        gmt_modified_milliseconds: str = None,
+        modifier_user_id: str = None,
+        record_inst_id: str = None,
+    ):
+        self.creator_user_id = creator_user_id
+        self.follow_content = follow_content
+        self.follow_target_data_id = follow_target_data_id
+        self.follow_target_type = follow_target_type
+        self.gmt_create_milliseconds = gmt_create_milliseconds
+        self.gmt_modified_milliseconds = gmt_modified_milliseconds
+        self.modifier_user_id = modifier_user_id
+        self.record_inst_id = record_inst_id
+
+    def validate(self):
+        if self.follow_content:
+            for k in self.follow_content:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.creator_user_id is not None:
+            result['creatorUserId'] = self.creator_user_id
+        result['followContent'] = []
+        if self.follow_content is not None:
+            for k in self.follow_content:
+                result['followContent'].append(k.to_map() if k else None)
+        if self.follow_target_data_id is not None:
+            result['followTargetDataId'] = self.follow_target_data_id
+        if self.follow_target_type is not None:
+            result['followTargetType'] = self.follow_target_type
+        if self.gmt_create_milliseconds is not None:
+            result['gmtCreateMilliseconds'] = self.gmt_create_milliseconds
+        if self.gmt_modified_milliseconds is not None:
+            result['gmtModifiedMilliseconds'] = self.gmt_modified_milliseconds
+        if self.modifier_user_id is not None:
+            result['modifierUserId'] = self.modifier_user_id
+        if self.record_inst_id is not None:
+            result['recordInstId'] = self.record_inst_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('creatorUserId') is not None:
+            self.creator_user_id = m.get('creatorUserId')
+        self.follow_content = []
+        if m.get('followContent') is not None:
+            for k in m.get('followContent'):
+                temp_model = FindTargetRelatedFollowRecordsResponseBodyResultResultListFollowContent()
+                self.follow_content.append(temp_model.from_map(k))
+        if m.get('followTargetDataId') is not None:
+            self.follow_target_data_id = m.get('followTargetDataId')
+        if m.get('followTargetType') is not None:
+            self.follow_target_type = m.get('followTargetType')
+        if m.get('gmtCreateMilliseconds') is not None:
+            self.gmt_create_milliseconds = m.get('gmtCreateMilliseconds')
+        if m.get('gmtModifiedMilliseconds') is not None:
+            self.gmt_modified_milliseconds = m.get('gmtModifiedMilliseconds')
+        if m.get('modifierUserId') is not None:
+            self.modifier_user_id = m.get('modifierUserId')
+        if m.get('recordInstId') is not None:
+            self.record_inst_id = m.get('recordInstId')
+        return self
+
+
+class FindTargetRelatedFollowRecordsResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        has_more: bool = None,
+        next_token: str = None,
+        result_list: List[FindTargetRelatedFollowRecordsResponseBodyResultResultList] = None,
+    ):
+        self.has_more = has_more
+        self.next_token = next_token
+        self.result_list = result_list
+
+    def validate(self):
+        if self.result_list:
+            for k in self.result_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        result['resultList'] = []
+        if self.result_list is not None:
+            for k in self.result_list:
+                result['resultList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        self.result_list = []
+        if m.get('resultList') is not None:
+            for k in m.get('resultList'):
+                temp_model = FindTargetRelatedFollowRecordsResponseBodyResultResultList()
+                self.result_list.append(temp_model.from_map(k))
+        return self
+
+
+class FindTargetRelatedFollowRecordsResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: FindTargetRelatedFollowRecordsResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = FindTargetRelatedFollowRecordsResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class FindTargetRelatedFollowRecordsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: FindTargetRelatedFollowRecordsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = FindTargetRelatedFollowRecordsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetAllCustomerRecyclesHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1503,14 +1503,104 @@
         self,
         request: dingtalktrip__1__0_models.SyncTripProductConfigRequest,
     ) -> dingtalktrip__1__0_models.SyncTripProductConfigResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalktrip__1__0_models.SyncTripProductConfigHeaders()
         return await self.sync_trip_product_config_with_options_async(request, headers, runtime)
 
+    def trip_platform_unified_entry_with_options(
+        self,
+        request: dingtalktrip__1__0_models.TripPlatformUnifiedEntryRequest,
+        headers: dingtalktrip__1__0_models.TripPlatformUnifiedEntryHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalktrip__1__0_models.TripPlatformUnifiedEntryResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.messages):
+            body['messages'] = request.messages
+        if not UtilClient.is_unset(request.method):
+            body['method'] = request.method
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='TripPlatformUnifiedEntry',
+            version='trip_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/trip/platforms/entrances/unify',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalktrip__1__0_models.TripPlatformUnifiedEntryResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def trip_platform_unified_entry_with_options_async(
+        self,
+        request: dingtalktrip__1__0_models.TripPlatformUnifiedEntryRequest,
+        headers: dingtalktrip__1__0_models.TripPlatformUnifiedEntryHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalktrip__1__0_models.TripPlatformUnifiedEntryResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.messages):
+            body['messages'] = request.messages
+        if not UtilClient.is_unset(request.method):
+            body['method'] = request.method
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='TripPlatformUnifiedEntry',
+            version='trip_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/trip/platforms/entrances/unify',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalktrip__1__0_models.TripPlatformUnifiedEntryResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def trip_platform_unified_entry(
+        self,
+        request: dingtalktrip__1__0_models.TripPlatformUnifiedEntryRequest,
+    ) -> dingtalktrip__1__0_models.TripPlatformUnifiedEntryResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalktrip__1__0_models.TripPlatformUnifiedEntryHeaders()
+        return self.trip_platform_unified_entry_with_options(request, headers, runtime)
+
+    async def trip_platform_unified_entry_async(
+        self,
+        request: dingtalktrip__1__0_models.TripPlatformUnifiedEntryRequest,
+    ) -> dingtalktrip__1__0_models.TripPlatformUnifiedEntryResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalktrip__1__0_models.TripPlatformUnifiedEntryHeaders()
+        return await self.trip_platform_unified_entry_with_options_async(request, headers, runtime)
+
     def upgrade_template_with_options(
         self,
         request: dingtalktrip__1__0_models.UpgradeTemplateRequest,
         headers: dingtalktrip__1__0_models.UpgradeTemplateHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalktrip__1__0_models.UpgradeTemplateResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3693,14 +3693,160 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SyncTripProductConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TripPlatformUnifiedEntryHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class TripPlatformUnifiedEntryRequest(TeaModel):
+    def __init__(
+        self,
+        messages: str = None,
+        method: str = None,
+    ):
+        self.messages = messages
+        self.method = method
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.messages is not None:
+            result['messages'] = self.messages
+        if self.method is not None:
+            result['method'] = self.method
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('messages') is not None:
+            self.messages = m.get('messages')
+        if m.get('method') is not None:
+            self.method = m.get('method')
+        return self
+
+
+class TripPlatformUnifiedEntryResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        result: str = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.result is not None:
+            result['result'] = self.result
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class TripPlatformUnifiedEntryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TripPlatformUnifiedEntryResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = TripPlatformUnifiedEntryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpgradeTemplateHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1315,14 +1315,104 @@
         return self.get_crm_proc_codes_with_options(headers, runtime)
 
     async def get_crm_proc_codes_async(self) -> dingtalkworkflow__1__0_models.GetCrmProcCodesResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkworkflow__1__0_models.GetCrmProcCodesHeaders()
         return await self.get_crm_proc_codes_with_options_async(headers, runtime)
 
+    def get_field_modified_history_with_options(
+        self,
+        request: dingtalkworkflow__1__0_models.GetFieldModifiedHistoryRequest,
+        headers: dingtalkworkflow__1__0_models.GetFieldModifiedHistoryHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.GetFieldModifiedHistoryResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.field_id):
+            body['fieldId'] = request.field_id
+        if not UtilClient.is_unset(request.process_instance_id):
+            body['processInstanceId'] = request.process_instance_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetFieldModifiedHistory',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/processes/fields/modifiedRecords/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.GetFieldModifiedHistoryResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_field_modified_history_with_options_async(
+        self,
+        request: dingtalkworkflow__1__0_models.GetFieldModifiedHistoryRequest,
+        headers: dingtalkworkflow__1__0_models.GetFieldModifiedHistoryHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.GetFieldModifiedHistoryResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.field_id):
+            body['fieldId'] = request.field_id
+        if not UtilClient.is_unset(request.process_instance_id):
+            body['processInstanceId'] = request.process_instance_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetFieldModifiedHistory',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/processes/fields/modifiedRecords/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.GetFieldModifiedHistoryResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_field_modified_history(
+        self,
+        request: dingtalkworkflow__1__0_models.GetFieldModifiedHistoryRequest,
+    ) -> dingtalkworkflow__1__0_models.GetFieldModifiedHistoryResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.GetFieldModifiedHistoryHeaders()
+        return self.get_field_modified_history_with_options(request, headers, runtime)
+
+    async def get_field_modified_history_async(
+        self,
+        request: dingtalkworkflow__1__0_models.GetFieldModifiedHistoryRequest,
+    ) -> dingtalkworkflow__1__0_models.GetFieldModifiedHistoryResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.GetFieldModifiedHistoryHeaders()
+        return await self.get_field_modified_history_with_options_async(request, headers, runtime)
+
     def get_manage_process_by_staff_id_with_options(
         self,
         request: dingtalkworkflow__1__0_models.GetManageProcessByStaffIdRequest,
         headers: dingtalkworkflow__1__0_models.GetManageProcessByStaffIdHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkworkflow__1__0_models.GetManageProcessByStaffIdResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3265,14 +3265,213 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetCrmProcCodesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetFieldModifiedHistoryHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetFieldModifiedHistoryRequest(TeaModel):
+    def __init__(
+        self,
+        field_id: str = None,
+        process_instance_id: str = None,
+    ):
+        self.field_id = field_id
+        self.process_instance_id = process_instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.field_id is not None:
+            result['fieldId'] = self.field_id
+        if self.process_instance_id is not None:
+            result['processInstanceId'] = self.process_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('fieldId') is not None:
+            self.field_id = m.get('fieldId')
+        if m.get('processInstanceId') is not None:
+            self.process_instance_id = m.get('processInstanceId')
+        return self
+
+
+class GetFieldModifiedHistoryResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        field_id: str = None,
+        name: str = None,
+        user_id: str = None,
+        value: str = None,
+    ):
+        self.create_time = create_time
+        self.field_id = field_id
+        self.name = name
+        self.user_id = user_id
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_time is not None:
+            result['createTime'] = self.create_time
+        if self.field_id is not None:
+            result['fieldId'] = self.field_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('createTime') is not None:
+            self.create_time = m.get('createTime')
+        if m.get('fieldId') is not None:
+            self.field_id = m.get('fieldId')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
+class GetFieldModifiedHistoryResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[GetFieldModifiedHistoryResponseBodyResult] = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = GetFieldModifiedHistoryResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class GetFieldModifiedHistoryResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetFieldModifiedHistoryResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetFieldModifiedHistoryResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetManageProcessByStaffIdHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -6695,23 +6894,25 @@
 
 
 class PagesExportInstancesResponseBodyResultListOperationRecords(TeaModel):
     def __init__(
         self,
         activity_id: str = None,
         attachments: List[PagesExportInstancesResponseBodyResultListOperationRecordsAttachments] = None,
+        images: List[str] = None,
         operation_type: str = None,
         remark: str = None,
         result: str = None,
         task_id: int = None,
         timestamp: int = None,
         user_id: str = None,
     ):
         self.activity_id = activity_id
         self.attachments = attachments
+        self.images = images
         self.operation_type = operation_type
         self.remark = remark
         self.result = result
         self.task_id = task_id
         self.timestamp = timestamp
         self.user_id = user_id
 
@@ -6729,14 +6930,16 @@
         result = dict()
         if self.activity_id is not None:
             result['activityId'] = self.activity_id
         result['attachments'] = []
         if self.attachments is not None:
             for k in self.attachments:
                 result['attachments'].append(k.to_map() if k else None)
+        if self.images is not None:
+            result['images'] = self.images
         if self.operation_type is not None:
             result['operationType'] = self.operation_type
         if self.remark is not None:
             result['remark'] = self.remark
         if self.result is not None:
             result['result'] = self.result
         if self.task_id is not None:
@@ -6752,14 +6955,16 @@
         if m.get('activityId') is not None:
             self.activity_id = m.get('activityId')
         self.attachments = []
         if m.get('attachments') is not None:
             for k in m.get('attachments'):
                 temp_model = PagesExportInstancesResponseBodyResultListOperationRecordsAttachments()
                 self.attachments.append(temp_model.from_map(k))
+        if m.get('images') is not None:
+            self.images = m.get('images')
         if m.get('operationType') is not None:
             self.operation_type = m.get('operationType')
         if m.get('remark') is not None:
             self.remark = m.get('remark')
         if m.get('result') is not None:
             self.result = m.get('result')
         if m.get('taskId') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6961,14 +6961,128 @@
         self,
         request: dingtalkyida__1__0_models.PageFormBaseInfosRequest,
     ) -> dingtalkyida__1__0_models.PageFormBaseInfosResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkyida__1__0_models.PageFormBaseInfosHeaders()
         return await self.page_form_base_infos_with_options_async(request, headers, runtime)
 
+    def preview_published_process_with_options(
+        self,
+        request: dingtalkyida__1__0_models.PreviewPublishedProcessRequest,
+        headers: dingtalkyida__1__0_models.PreviewPublishedProcessHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkyida__1__0_models.PreviewPublishedProcessResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_type):
+            body['appType'] = request.app_type
+        if not UtilClient.is_unset(request.department_id):
+            body['departmentId'] = request.department_id
+        if not UtilClient.is_unset(request.form_data_json):
+            body['formDataJson'] = request.form_data_json
+        if not UtilClient.is_unset(request.form_uuid):
+            body['formUuid'] = request.form_uuid
+        if not UtilClient.is_unset(request.language):
+            body['language'] = request.language
+        if not UtilClient.is_unset(request.process_code):
+            body['processCode'] = request.process_code
+        if not UtilClient.is_unset(request.system_token):
+            body['systemToken'] = request.system_token
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PreviewPublishedProcess',
+            version='yida_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/yida/processes/preview',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkyida__1__0_models.PreviewPublishedProcessResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def preview_published_process_with_options_async(
+        self,
+        request: dingtalkyida__1__0_models.PreviewPublishedProcessRequest,
+        headers: dingtalkyida__1__0_models.PreviewPublishedProcessHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkyida__1__0_models.PreviewPublishedProcessResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_type):
+            body['appType'] = request.app_type
+        if not UtilClient.is_unset(request.department_id):
+            body['departmentId'] = request.department_id
+        if not UtilClient.is_unset(request.form_data_json):
+            body['formDataJson'] = request.form_data_json
+        if not UtilClient.is_unset(request.form_uuid):
+            body['formUuid'] = request.form_uuid
+        if not UtilClient.is_unset(request.language):
+            body['language'] = request.language
+        if not UtilClient.is_unset(request.process_code):
+            body['processCode'] = request.process_code
+        if not UtilClient.is_unset(request.system_token):
+            body['systemToken'] = request.system_token
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PreviewPublishedProcess',
+            version='yida_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/yida/processes/preview',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkyida__1__0_models.PreviewPublishedProcessResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def preview_published_process(
+        self,
+        request: dingtalkyida__1__0_models.PreviewPublishedProcessRequest,
+    ) -> dingtalkyida__1__0_models.PreviewPublishedProcessResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkyida__1__0_models.PreviewPublishedProcessHeaders()
+        return self.preview_published_process_with_options(request, headers, runtime)
+
+    async def preview_published_process_async(
+        self,
+        request: dingtalkyida__1__0_models.PreviewPublishedProcessRequest,
+    ) -> dingtalkyida__1__0_models.PreviewPublishedProcessResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkyida__1__0_models.PreviewPublishedProcessHeaders()
+        return await self.preview_published_process_with_options_async(request, headers, runtime)
+
     def query_service_record_with_options(
         self,
         request: dingtalkyida__1__0_models.QueryServiceRecordRequest,
         headers: dingtalkyida__1__0_models.QueryServiceRecordHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkyida__1__0_models.QueryServiceRecordResponse:
         UtilClient.validate_model(request)
@@ -9175,14 +9289,16 @@
             body['formDataJson'] = request.form_data_json
         if not UtilClient.is_unset(request.form_uuid):
             body['formUuid'] = request.form_uuid
         if not UtilClient.is_unset(request.language):
             body['language'] = request.language
         if not UtilClient.is_unset(request.process_code):
             body['processCode'] = request.process_code
+        if not UtilClient.is_unset(request.process_data):
+            body['processData'] = request.process_data
         if not UtilClient.is_unset(request.system_token):
             body['systemToken'] = request.system_token
         if not UtilClient.is_unset(request.user_id):
             body['userId'] = request.user_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -9224,14 +9340,16 @@
             body['formDataJson'] = request.form_data_json
         if not UtilClient.is_unset(request.form_uuid):
             body['formUuid'] = request.form_uuid
         if not UtilClient.is_unset(request.language):
             body['language'] = request.language
         if not UtilClient.is_unset(request.process_code):
             body['processCode'] = request.process_code
+        if not UtilClient.is_unset(request.process_data):
+            body['processData'] = request.process_data
         if not UtilClient.is_unset(request.system_token):
             body['systemToken'] = request.system_token
         if not UtilClient.is_unset(request.user_id):
             body['userId'] = request.user_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -15534,14 +15534,363 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PageFormBaseInfosResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PreviewPublishedProcessHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class PreviewPublishedProcessRequest(TeaModel):
+    def __init__(
+        self,
+        app_type: str = None,
+        department_id: str = None,
+        form_data_json: str = None,
+        form_uuid: str = None,
+        language: str = None,
+        process_code: str = None,
+        system_token: str = None,
+        user_id: str = None,
+    ):
+        self.app_type = app_type
+        self.department_id = department_id
+        self.form_data_json = form_data_json
+        self.form_uuid = form_uuid
+        self.language = language
+        self.process_code = process_code
+        self.system_token = system_token
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_type is not None:
+            result['appType'] = self.app_type
+        if self.department_id is not None:
+            result['departmentId'] = self.department_id
+        if self.form_data_json is not None:
+            result['formDataJson'] = self.form_data_json
+        if self.form_uuid is not None:
+            result['formUuid'] = self.form_uuid
+        if self.language is not None:
+            result['language'] = self.language
+        if self.process_code is not None:
+            result['processCode'] = self.process_code
+        if self.system_token is not None:
+            result['systemToken'] = self.system_token
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('appType') is not None:
+            self.app_type = m.get('appType')
+        if m.get('departmentId') is not None:
+            self.department_id = m.get('departmentId')
+        if m.get('formDataJson') is not None:
+            self.form_data_json = m.get('formDataJson')
+        if m.get('formUuid') is not None:
+            self.form_uuid = m.get('formUuid')
+        if m.get('language') is not None:
+            self.language = m.get('language')
+        if m.get('processCode') is not None:
+            self.process_code = m.get('processCode')
+        if m.get('systemToken') is not None:
+            self.system_token = m.get('systemToken')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class PreviewPublishedProcessResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        action: str = None,
+        action_exit: str = None,
+        active_time_gmt: str = None,
+        activity_id: str = None,
+        data_id: int = None,
+        digital_sign: str = None,
+        domains: List[Any] = None,
+        files: str = None,
+        operate_time_gmt: str = None,
+        operate_type: str = None,
+        operator_display_name: str = None,
+        operator_name: str = None,
+        operator_nick_name: str = None,
+        operator_photo_url: str = None,
+        operator_status: str = None,
+        operator_user_id: str = None,
+        process_instance_id: str = None,
+        remark: str = None,
+        show_name: str = None,
+        size: int = None,
+        task_execute_type: str = None,
+        task_hold_time_gmt: int = None,
+        task_id: str = None,
+        task_type: str = None,
+        type: str = None,
+    ):
+        self.action = action
+        self.action_exit = action_exit
+        self.active_time_gmt = active_time_gmt
+        self.activity_id = activity_id
+        self.data_id = data_id
+        self.digital_sign = digital_sign
+        self.domains = domains
+        self.files = files
+        self.operate_time_gmt = operate_time_gmt
+        self.operate_type = operate_type
+        self.operator_display_name = operator_display_name
+        self.operator_name = operator_name
+        self.operator_nick_name = operator_nick_name
+        self.operator_photo_url = operator_photo_url
+        self.operator_status = operator_status
+        self.operator_user_id = operator_user_id
+        self.process_instance_id = process_instance_id
+        self.remark = remark
+        self.show_name = show_name
+        self.size = size
+        self.task_execute_type = task_execute_type
+        self.task_hold_time_gmt = task_hold_time_gmt
+        self.task_id = task_id
+        self.task_type = task_type
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action is not None:
+            result['action'] = self.action
+        if self.action_exit is not None:
+            result['actionExit'] = self.action_exit
+        if self.active_time_gmt is not None:
+            result['activeTimeGMT'] = self.active_time_gmt
+        if self.activity_id is not None:
+            result['activityId'] = self.activity_id
+        if self.data_id is not None:
+            result['dataId'] = self.data_id
+        if self.digital_sign is not None:
+            result['digitalSign'] = self.digital_sign
+        if self.domains is not None:
+            result['domains'] = self.domains
+        if self.files is not None:
+            result['files'] = self.files
+        if self.operate_time_gmt is not None:
+            result['operateTimeGMT'] = self.operate_time_gmt
+        if self.operate_type is not None:
+            result['operateType'] = self.operate_type
+        if self.operator_display_name is not None:
+            result['operatorDisplayName'] = self.operator_display_name
+        if self.operator_name is not None:
+            result['operatorName'] = self.operator_name
+        if self.operator_nick_name is not None:
+            result['operatorNickName'] = self.operator_nick_name
+        if self.operator_photo_url is not None:
+            result['operatorPhotoUrl'] = self.operator_photo_url
+        if self.operator_status is not None:
+            result['operatorStatus'] = self.operator_status
+        if self.operator_user_id is not None:
+            result['operatorUserId'] = self.operator_user_id
+        if self.process_instance_id is not None:
+            result['processInstanceId'] = self.process_instance_id
+        if self.remark is not None:
+            result['remark'] = self.remark
+        if self.show_name is not None:
+            result['showName'] = self.show_name
+        if self.size is not None:
+            result['size'] = self.size
+        if self.task_execute_type is not None:
+            result['taskExecuteType'] = self.task_execute_type
+        if self.task_hold_time_gmt is not None:
+            result['taskHoldTimeGMT'] = self.task_hold_time_gmt
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        if self.task_type is not None:
+            result['taskType'] = self.task_type
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('action') is not None:
+            self.action = m.get('action')
+        if m.get('actionExit') is not None:
+            self.action_exit = m.get('actionExit')
+        if m.get('activeTimeGMT') is not None:
+            self.active_time_gmt = m.get('activeTimeGMT')
+        if m.get('activityId') is not None:
+            self.activity_id = m.get('activityId')
+        if m.get('dataId') is not None:
+            self.data_id = m.get('dataId')
+        if m.get('digitalSign') is not None:
+            self.digital_sign = m.get('digitalSign')
+        if m.get('domains') is not None:
+            self.domains = m.get('domains')
+        if m.get('files') is not None:
+            self.files = m.get('files')
+        if m.get('operateTimeGMT') is not None:
+            self.operate_time_gmt = m.get('operateTimeGMT')
+        if m.get('operateType') is not None:
+            self.operate_type = m.get('operateType')
+        if m.get('operatorDisplayName') is not None:
+            self.operator_display_name = m.get('operatorDisplayName')
+        if m.get('operatorName') is not None:
+            self.operator_name = m.get('operatorName')
+        if m.get('operatorNickName') is not None:
+            self.operator_nick_name = m.get('operatorNickName')
+        if m.get('operatorPhotoUrl') is not None:
+            self.operator_photo_url = m.get('operatorPhotoUrl')
+        if m.get('operatorStatus') is not None:
+            self.operator_status = m.get('operatorStatus')
+        if m.get('operatorUserId') is not None:
+            self.operator_user_id = m.get('operatorUserId')
+        if m.get('processInstanceId') is not None:
+            self.process_instance_id = m.get('processInstanceId')
+        if m.get('remark') is not None:
+            self.remark = m.get('remark')
+        if m.get('showName') is not None:
+            self.show_name = m.get('showName')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        if m.get('taskExecuteType') is not None:
+            self.task_execute_type = m.get('taskExecuteType')
+        if m.get('taskHoldTimeGMT') is not None:
+            self.task_hold_time_gmt = m.get('taskHoldTimeGMT')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        if m.get('taskType') is not None:
+            self.task_type = m.get('taskType')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class PreviewPublishedProcessResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[PreviewPublishedProcessResponseBodyResult] = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = PreviewPublishedProcessResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        return self
+
+
+class PreviewPublishedProcessResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PreviewPublishedProcessResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = PreviewPublishedProcessResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryServiceRecordHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -20051,23 +20400,25 @@
         self,
         app_type: str = None,
         department_id: str = None,
         form_data_json: str = None,
         form_uuid: str = None,
         language: str = None,
         process_code: str = None,
+        process_data: str = None,
         system_token: str = None,
         user_id: str = None,
     ):
         self.app_type = app_type
         self.department_id = department_id
         self.form_data_json = form_data_json
         self.form_uuid = form_uuid
         self.language = language
         self.process_code = process_code
+        self.process_data = process_data
         self.system_token = system_token
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -20084,14 +20435,16 @@
             result['formDataJson'] = self.form_data_json
         if self.form_uuid is not None:
             result['formUuid'] = self.form_uuid
         if self.language is not None:
             result['language'] = self.language
         if self.process_code is not None:
             result['processCode'] = self.process_code
+        if self.process_data is not None:
+            result['processData'] = self.process_data
         if self.system_token is not None:
             result['systemToken'] = self.system_token
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
@@ -20104,14 +20457,16 @@
             self.form_data_json = m.get('formDataJson')
         if m.get('formUuid') is not None:
             self.form_uuid = m.get('formUuid')
         if m.get('language') is not None:
             self.language = m.get('language')
         if m.get('processCode') is not None:
             self.process_code = m.get('processCode')
+        if m.get('processData') is not None:
+            self.process_data = m.get('processData')
         if m.get('systemToken') is not None:
             self.system_token = m.get('systemToken')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.94
+Version: 2.0.95
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.95/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 alibabacloud_dingtalk/ai_paa_s_1_0/models.py
 alibabacloud_dingtalk/algo_1_0/__init__.py
 alibabacloud_dingtalk/algo_1_0/client.py
 alibabacloud_dingtalk/algo_1_0/models.py
 alibabacloud_dingtalk/alitrip_1_0/__init__.py
 alibabacloud_dingtalk/alitrip_1_0/client.py
 alibabacloud_dingtalk/alitrip_1_0/models.py
+alibabacloud_dingtalk/amdp_1_0/__init__.py
+alibabacloud_dingtalk/amdp_1_0/client.py
+alibabacloud_dingtalk/amdp_1_0/models.py
 alibabacloud_dingtalk/apaas_1_0/__init__.py
 alibabacloud_dingtalk/apaas_1_0/client.py
 alibabacloud_dingtalk/apaas_1_0/models.py
 alibabacloud_dingtalk/app_market_1_0/__init__.py
 alibabacloud_dingtalk/app_market_1_0/client.py
 alibabacloud_dingtalk/app_market_1_0/models.py
 alibabacloud_dingtalk/ats_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.0.94/setup.py` & `alibabacloud_dingtalk-2.0.95/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 09/04/2024
+Created on 15/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

