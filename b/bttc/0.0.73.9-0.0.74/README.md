# Comparing `tmp/bttc-0.0.73.9.tar.gz` & `tmp/bttc-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.73.9.tar", last modified: Wed Apr 10 07:52:08 2024, max compression
+gzip compressed data, was "bttc-0.0.74.tar", last modified: Mon Apr 15 06:19:09 2024, max compression
```

## Comparing `bttc-0.0.73.9.tar` & `bttc-0.0.74.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.955250 bttc-0.0.73.9/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73.9/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 07:52:08.955250 bttc-0.0.73.9/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-08 13:33:17.000000 bttc-0.0.73.9/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5315 2024-04-10 07:51:36.000000 bttc-0.0.73.9/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-09 04:28:05.000000 bttc-0.0.73.9/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.73.9/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16265 2024-04-10 05:57:16.000000 bttc-0.0.73.9/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.73.9/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22487 2024-04-10 07:45:43.000000 bttc-0.0.73.9/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.73.9/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/general_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.947250 bttc-0.0.73.9/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.955250 bttc-0.0.73.9/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.955250 bttc-0.0.73.9/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3909 2024-04-10 07:48:22.000000 bttc-0.0.73.9/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.955250 bttc-0.0.73.9/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/logcat.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/utils/typing_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-08 13:33:17.000000 bttc-0.0.73.9/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73.9/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-10 07:52:08.951250 bttc-0.0.73.9/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-10 07:52:08.000000 bttc-0.0.73.9/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-10 07:52:08.955250 bttc-0.0.73.9/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-10 00:48:38.000000 bttc-0.0.73.9/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.732741 bttc-0.0.74/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.74/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2135 2024-04-15 06:19:09.732741 bttc-0.0.74/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1407 2024-04-15 06:18:54.000000 bttc-0.0.74/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.728741 bttc-0.0.74/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5313 2024-04-15 06:15:48.000000 bttc-0.0.74/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.74/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.74/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16265 2024-04-15 06:13:29.000000 bttc-0.0.74/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.728741 bttc-0.0.74/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.74/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:14:44.000000 bttc-0.0.74/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-04-08 13:33:17.000000 bttc-0.0.74/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/general_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.728741 bttc-0.0.74/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.728741 bttc-0.0.74/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.724741 bttc-0.0.74/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.728741 bttc-0.0.74/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.728741 bttc-0.0.74/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.728741 bttc-0.0.74/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.74/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.732741 bttc-0.0.74/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/utils/logcat.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/utils/typing_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2915 2024-04-15 06:13:29.000000 bttc-0.0.74/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.74/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-15 06:19:09.728741 bttc-0.0.74/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2135 2024-04-15 06:19:09.000000 bttc-0.0.74/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1284 2024-04-15 06:19:09.000000 bttc-0.0.74/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-15 06:19:09.000000 bttc-0.0.74/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-04-15 06:19:09.000000 bttc-0.0.74/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-15 06:19:09.000000 bttc-0.0.74/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-15 06:19:09.732741 bttc-0.0.74/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1714 2024-04-15 06:13:29.000000 bttc-0.0.74/setup.py
```

### Comparing `bttc-0.0.73.9/LICENSE` & `bttc-0.0.74/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/PKG-INFO` & `bttc-0.0.74/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.9
+Version: 0.0.74
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,14 +61,15 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
```

### Comparing `bttc-0.0.73.9/README.md` & `bttc-0.0.74/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
```

### Comparing `bttc-0.0.73.9/bttc/__init__.py` & `bttc-0.0.74/bttc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from bttc import errors
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 from typing import TypeAlias
 
 
-__version__ = '0.0.73.9'
+__version__ = '0.0.74'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.73.9/bttc/apk_utils.py` & `bttc-0.0.74/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/ble_data.py` & `bttc-0.0.74/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/ble_utils.py` & `bttc-0.0.74/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/bt_data.py` & `bttc-0.0.74/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/bt_utils.py` & `bttc-0.0.74/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/cli/__init__.py` & `bttc-0.0.74/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/cli/constants.py` & `bttc-0.0.74/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/cli/main.py` & `bttc-0.0.74/bttc/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,18 @@
 select_parser = cmd2.Cmd2ArgumentParser()
 select_parser.add_argument(
     '-s', '--serial', type=str, default=None, help='DUT serial')
 
 logcat_filter_parser = cmd2.Cmd2ArgumentParser()
 logcat_filter_parser.add_argument(
     '--logcat_wait_sec', type=int, default=10,
-    help='Time in sec to follow logcat.')
+    help='Time in sec to follow logcat. (10s as default)')
 logcat_filter_parser.add_argument(
     '--logcat_only_match', type=bool, default=False,
-    help='Setup to show only matched line')
+    help='Setup to show only matched line. (False as default)')
 
 load_cmd2_commandset_parser = cmd2.Cmd2ArgumentParser()
 load_cmd2_commandset_parser.add_argument(
     '-p', '--cmd2_module_path', type=str, default=None,
     help='Cmd2 module path where holds command set class.')
 
 
@@ -443,16 +443,17 @@
     for path in dump_path_list:
       self._app.poutput(f'Dump UI page to {path}...\n')
       self._app._dut.gm.get_ui_xml(path)
 
     print('')
 
 
+@cmd2.with_default_category('Main')
 class BttcCmdApp(cmd2.Cmd):
-  """BTTC  cmd2 application."""
+  """BTTC cmd2 application."""
   MAIN_PROMPT = f'{Color.BOLD}{Color.BLUE}bttc>{Color.END} '
   DEVICE_PROMPT_PROMPT = (
       f'{Color.BOLD}{Color.BLUE}bttc/{Color.YELLOW}' + r'{serial}' +
       Color.BLINK_SLOW + '> ' + Color.END)
 
   def __init__(self, serial: str | None = None):
     super().__init__(
@@ -517,14 +518,15 @@
     """Loads SL4A service in DUT."""
     device_factory.load_sl4a(self._dut)
     self.dut_init_sl4a = True
 
   @dec_require_dut
   @cmd2.with_argparser(logcat_filter_parser)
   def do_logcat_filter(self, args):
+    """Filters message in logcat."""
     pattern_list = []
     while True:
       try:
         pattern_str = self.read_input(
             "Pattern (enter nothing to stop)? ",
             history=self.logcat_pattern_history,
             completion_mode=cmd2.CompletionMode.CUSTOM).strip()
```

### Comparing `bttc-0.0.73.9/bttc/common_data.py` & `bttc-0.0.74/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/constants.py` & `bttc-0.0.74/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/core.py` & `bttc-0.0.74/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/errors.py` & `bttc-0.0.74/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/general_utils.py` & `bttc-0.0.74/bttc/general_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.74/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.74/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.74/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.74/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.74/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.74/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.74/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/avrcp/errors.py` & `bttc-0.0.74/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/hfp/__init__.py` & `bttc-0.0.74/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/hfp/constants.py` & `bttc-0.0.74/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/hfp/errors.py` & `bttc-0.0.74/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.74/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.74/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.74/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.74/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/strategy.py` & `bttc-0.0.74/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/utils/ad_checker.py` & `bttc-0.0.74/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/utils/device_factory.py` & `bttc-0.0.74/bttc/utils/device_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 from bttc.mobly_android_device_lib import tl4a_snippet_client
 from bttc.mobly_android_device_lib.services import sl4a_service
 
 from snippet_uiautomator import uiautomator
 from typing import Any, Callable, TypeAlias, Union
 
 
+AnyCallable: TypeAlias = Callable[..., Any]
 GeneralDevice: TypeAlias = android_device.AndroidDevice
 
 
-def dec_depress_ex(do_depress: bool = False) -> Callable[Any, ...]:
-  def inner(func: Callable[Any, ...]) -> Callable[Any, ...]:
+def dec_depress_ex(do_depress: bool = False) -> AnyCallable:
+  def inner(func: AnyCallable) -> AnyCallable:
     def wrapper(*args, **kwargs):
       try:
         func(*args, **kwargs)
       except Exception as ex:
         if do_depress:
           logging.warning('%s', ex)
         else:
```

### Comparing `bttc-0.0.73.9/bttc/utils/iperf/__init__.py` & `bttc-0.0.74/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/utils/iperf/errors.py` & `bttc-0.0.74/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/utils/key_events_handler.py` & `bttc-0.0.74/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/utils/log_parser.py` & `bttc-0.0.74/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/utils/logcat.py` & `bttc-0.0.74/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/utils/retry.py` & `bttc-0.0.74/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/utils/typing_utils.py` & `bttc-0.0.74/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/utils_loader.py` & `bttc-0.0.74/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc/wifi_utils.py` & `bttc-0.0.74/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/bttc.egg-info/PKG-INFO` & `bttc-0.0.74/bttc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.73.9
+Version: 0.0.74
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,14 +61,15 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
```

### Comparing `bttc-0.0.73.9/bttc.egg-info/SOURCES.txt` & `bttc-0.0.74/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.73.9/setup.py` & `bttc-0.0.74/setup.py`

 * *Files identical despite different names*

