# Comparing `tmp/waylay_sdk_storage_types-0.4.1.20240415.tar.gz` & `tmp/waylay-sdk-storage-types-0.4.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_storage_types-0.4.1.20240415.tar", last modified: Mon Apr 15 08:21:02 2024, max compression
+gzip compressed data, was "waylay-sdk-storage-types-0.4.1b1.tar", last modified: Thu Mar 28 13:32:40 2024, max compression
```

## Comparing `waylay_sdk_storage_types-0.4.1.20240415.tar` & `waylay-sdk-storage-types-0.4.1b1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:02.033124 waylay_sdk_storage_types-0.4.1.20240415/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-15 08:21:02.033124 waylay_sdk_storage_types-0.4.1.20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:21:02.033124 waylay_sdk_storage_types-0.4.1.20240415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:02.021124 waylay_sdk_storage_types-0.4.1.20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:02.021124 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:02.021124 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:02.021124 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:02.029124 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/authentication_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket_object_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucketcreationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucketpolicystatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/channeltype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/event_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/expiry.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/hal_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/httpmethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/location_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/notification_queue_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/notification_queue_status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/payload_config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/queuesetupstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/sign.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/store.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/storetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/subscription_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/subscriptions_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/system_channel_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/system_channel_config_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/tenant_status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/venttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/web_script_channel_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/web_script_channel_config_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:02.029124 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/bucket_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-15 08:20:55.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/subscription_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:21:02.033124 waylay_sdk_storage_types-0.4.1.20240415/src/waylay_sdk_storage_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-15 08:21:02.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay_sdk_storage_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-15 08:21:02.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay_sdk_storage_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:21:02.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay_sdk_storage_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-15 08:21:02.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay_sdk_storage_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 08:21:02.000000 waylay_sdk_storage_types-0.4.1.20240415/src/waylay_sdk_storage_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.865666 waylay-sdk-storage-types-0.4.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-28 13:32:40.865666 waylay-sdk-storage-types-0.4.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:32:40.865666 waylay-sdk-storage-types-0.4.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.853666 waylay-sdk-storage-types-0.4.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.853666 waylay-sdk-storage-types-0.4.1b1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.853666 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.853666 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.861666 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/authentication_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_object_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucketcreationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucketpolicystatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/channeltype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/expiry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/hal_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/httpmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/location_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/notification_queue_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/notification_queue_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/payload_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/queuesetupstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/storetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscription_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscriptions_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/system_channel_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/system_channel_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/tenant_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/venttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/web_script_channel_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/web_script_channel_config_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.861666 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/about_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/bucket_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/subscription_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.861666 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/LICENSE.txt` & `waylay-sdk-storage-types-0.4.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/PKG-INFO` & `waylay-sdk-storage-types-0.4.1b1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage-types
-Version: 0.4.1.20240415
+Version: 0.4.1b1
 Summary: Waylay Storage Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
-Requires-Dist: waylay-sdk-storage==0.4.1.20240415
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-storage==0.4.1b1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,57 +46,49 @@
 
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
 It is considered an extension of the waylay-sdk-storage package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-storage`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
-from waylay.services.storage.models.tenant_status_report import TenantStatusReport
 try:
-    # Status
-    # calls `GET /storage/v1/status`
-    api_response = await waylay_client.storage.about.status(
-        # query parameters:
-        query = {
-            'include_buckets': True
-            'include_queues': True
-            'include_disk_usage': False
-        },
+    # Version
+    # calls `GET /storage/v1/`
+    api_response = await waylay_client.storage.about.version(
     )
-    print("The response of storage.about.status:\n")
+    print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling storage.about.status: %s\n" % e)
+    print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/README.md` & `waylay-sdk-storage-types-0.4.1b1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
 It is considered an extension of the waylay-sdk-storage package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-storage`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
-from waylay.services.storage.models.tenant_status_report import TenantStatusReport
 try:
-    # Status
-    # calls `GET /storage/v1/status`
-    api_response = await waylay_client.storage.about.status(
-        # query parameters:
-        query = {
-            'include_buckets': True
-            'include_queues': True
-            'include_disk_usage': False
-        },
+    # Version
+    # calls `GET /storage/v1/`
+    api_response = await waylay_client.storage.about.version(
     )
-    print("The response of storage.about.status:\n")
+    print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling storage.about.status: %s\n" % e)
+    print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/pyproject.toml` & `waylay-sdk-storage-types-0.4.1b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-storage-types"
-version = "0.4.1.20240415"
+version = "0.4.1b1"
 description = "Waylay Storage Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Storage" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.0",
-    "waylay-sdk-storage == 0.4.1.20240415",
+    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-storage == 0.4.1b1",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-storage-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/storage.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/__init__.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # coding: utf-8
 """Waylay Storage: REST Models.
 
 This code was generated from the OpenAPI documentation of 'Waylay Storage'
 
-version: 0.4.1
+version: v0.4.1
 
  Manage storage buckets and subscriptions.
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "0.4.1.20240415"
+__version__ = "0.4.1b1"
 
 # import models into model package
 from .auth import AUTH
 from .authentication_config import AuthenticationConfig
 from .bucket import Bucket
 from .bucket_configuration import BucketConfiguration
 from .bucket_listing import BucketListing
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/auth.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/auth.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/authentication_config.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/authentication_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket_configuration.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_configuration.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket_listing.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket_object.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_object.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucket_object_listing.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_object_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucketcreationstatus.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucketcreationstatus.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/bucketpolicystatus.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucketpolicystatus.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/channel.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/channel.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/event_filter.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/event_filter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/expiry.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/expiry.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/hal_entity.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/hal_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/hal_link.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/http_validation_error.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/notification_queue_status.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/notification_queue_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/notification_queue_status_report.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/notification_queue_status_report.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/payload_config.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/payload_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/queuesetupstatus.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/queuesetupstatus.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/response_list.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/response_list.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/store.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/store.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/subscription_config.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscription_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/subscriptions.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscriptions.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/subscriptions_listing.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscriptions_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/system_channel_config.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/system_channel_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/tenant_status_report.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/tenant_status_report.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/validation_error.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/models/web_script_channel_config.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/web_script_channel_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/about_api.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/about_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,14 @@
     ConfigDict,
     StrictBool,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-def _get_query_alias_for(field_name: str) -> str:
-    return field_name
-
-
-class GetQuery(WaylayBaseModel):
-    """Model for `get` query parameters."""
-
-    model_config = ConfigDict(
-        validate_assignment=True,
-        protected_namespaces=(),
-        extra="allow",
-        alias_generator=_get_query_alias_for,
-        populate_by_name=True,
-    )
-
-
 def _status_query_alias_for(field_name: str) -> str:
     if field_name == "store":
         return "store"
     if field_name == "include_buckets":
         return "include_buckets"
     if field_name == "include_queues":
         return "include_queues"
@@ -57,7 +41,23 @@
     model_config = ConfigDict(
         validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_status_query_alias_for,
         populate_by_name=True,
     )
+
+
+def _version_query_alias_for(field_name: str) -> str:
+    return field_name
+
+
+class VersionQuery(WaylayBaseModel):
+    """Model for `version` query parameters."""
+
+    model_config = ConfigDict(
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
+        alias_generator=_version_query_alias_for,
+        populate_by_name=True,
+    )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/bucket_api.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/bucket_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/object_api.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/object_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay/services/storage/queries/subscription_api.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/subscription_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay_sdk_storage_types.egg-info/PKG-INFO` & `waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage-types
-Version: 0.4.1.20240415
+Version: 0.4.1b1
 Summary: Waylay Storage Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
-Requires-Dist: waylay-sdk-storage==0.4.1.20240415
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-storage==0.4.1b1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,57 +46,49 @@
 
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
 It is considered an extension of the waylay-sdk-storage package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-storage`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
-from waylay.services.storage.models.tenant_status_report import TenantStatusReport
 try:
-    # Status
-    # calls `GET /storage/v1/status`
-    api_response = await waylay_client.storage.about.status(
-        # query parameters:
-        query = {
-            'include_buckets': True
-            'include_queues': True
-            'include_disk_usage': False
-        },
+    # Version
+    # calls `GET /storage/v1/`
+    api_response = await waylay_client.storage.about.version(
     )
-    print("The response of storage.about.status:\n")
+    print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling storage.about.status: %s\n" % e)
+    print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240415/src/waylay_sdk_storage_types.egg-info/SOURCES.txt` & `waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

