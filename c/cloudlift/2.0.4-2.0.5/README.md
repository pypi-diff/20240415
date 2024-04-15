# Comparing `tmp/cloudlift-2.0.4.tar.gz` & `tmp/cloudlift-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlift-2.0.4.tar", last modified: Thu Nov  2 07:53:49 2023, max compression
+gzip compressed data, was "cloudlift-2.0.5.tar", last modified: Mon Apr 15 15:46:14 2024, max compression
```

## Comparing `cloudlift-2.0.4.tar` & `cloudlift-2.0.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-11-02 07:53:49.434929 cloudlift-2.0.4/
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1062 2020-04-14 13:38:03.000000 cloudlift-2.0.4/LICENSE
--rwxrwxrwx   0 shoan     (1000) shoan     (1000)       40 2020-02-21 06:48:18.000000 cloudlift-2.0.4/MANIFEST.in
--rw-r--r--   0 shoan     (1000) shoan     (1000)    13573 2023-11-02 07:53:49.431632 cloudlift-2.0.4/PKG-INFO
--rw-r--r--   0 shoan     (1000) shoan     (1000)    13309 2023-10-03 12:20:25.000000 cloudlift-2.0.4/README.md
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-11-02 07:53:48.352352 cloudlift-2.0.4/cloudlift/
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6400 2023-04-26 12:53:28.000000 cloudlift-2.0.4/cloudlift/__init__.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-11-02 07:53:48.855354 cloudlift-2.0.4/cloudlift/config/
--rw-r--r--   0 shoan     (1000) shoan     (1000)      266 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/config/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      669 2023-02-02 12:14:14.000000 cloudlift-2.0.4/cloudlift/config/account.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      448 2023-02-02 08:10:32.000000 cloudlift-2.0.4/cloudlift/config/banner.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      621 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/config/decimal_encoder.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     2408 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/config/diff.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     1844 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/config/dynamodb_configuration.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    22093 2023-10-18 05:44:39.000000 cloudlift-2.0.4/cloudlift/config/environment_configuration.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      546 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/config/logging.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     2129 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/config/mfa.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     4387 2023-01-25 11:43:34.000000 cloudlift-2.0.4/cloudlift/config/parameter_store.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     2568 2023-04-26 12:53:28.000000 cloudlift-2.0.4/cloudlift/config/pre_flight.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     3516 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/config/region.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    20176 2023-10-18 05:44:39.000000 cloudlift-2.0.4/cloudlift/config/service_configuration.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      161 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/config/stack.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     7127 2023-10-03 12:20:25.000000 cloudlift-2.0.4/cloudlift/config/utils.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      217 2023-10-03 12:20:25.000000 cloudlift-2.0.4/cloudlift/constants.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-11-02 07:53:49.242287 cloudlift-2.0.4/cloudlift/deployment/
--rw-r--r--   0 shoan     (1000) shoan     (1000)      373 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/deployment/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     3154 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/deployment/changesets.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    41735 2023-10-18 05:44:40.000000 cloudlift-2.0.4/cloudlift/deployment/cluster_template_generator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      267 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/deployment/configs.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6391 2023-07-18 05:11:33.000000 cloudlift-2.0.4/cloudlift/deployment/deployer.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6981 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/deployment/ecr_client.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    18003 2023-10-11 11:27:13.000000 cloudlift-2.0.4/cloudlift/deployment/ecs.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      996 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/deployment/editor.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     8032 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/deployment/environment_creator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      896 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/deployment/progress.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6646 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/deployment/service_creator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     7056 2023-10-03 12:20:25.000000 cloudlift-2.0.4/cloudlift/deployment/service_information_fetcher.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    46514 2023-10-11 11:27:13.000000 cloudlift-2.0.4/cloudlift/deployment/service_template_generator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     4397 2023-02-02 08:10:32.000000 cloudlift-2.0.4/cloudlift/deployment/service_updater.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6527 2023-04-26 12:53:28.000000 cloudlift-2.0.4/cloudlift/deployment/task_definition_creator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     1257 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/deployment/template_generator.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-11-02 07:53:49.290287 cloudlift-2.0.4/cloudlift/exceptions/
--rw-r--r--   0 shoan     (1000) shoan     (1000)       46 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/exceptions/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      154 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/exceptions/exceptions.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-11-02 07:53:49.336291 cloudlift-2.0.4/cloudlift/session/
--rw-r--r--   0 shoan     (1000) shoan     (1000)       30 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/session/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     1874 2022-12-15 11:12:05.000000 cloudlift-2.0.4/cloudlift/session/session_creator.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-11-02 07:53:49.359241 cloudlift-2.0.4/cloudlift/version/
--rw-r--r--   0 shoan     (1000) shoan     (1000)       17 2023-10-18 05:44:40.000000 cloudlift-2.0.4/cloudlift/version/__init__.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-11-02 07:53:48.486538 cloudlift-2.0.4/cloudlift.egg-info/
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)    13573 2023-11-02 07:53:47.000000 cloudlift-2.0.4/cloudlift.egg-info/PKG-INFO
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1665 2023-11-02 07:53:48.000000 cloudlift-2.0.4/cloudlift.egg-info/SOURCES.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2023-11-02 07:53:47.000000 cloudlift-2.0.4/cloudlift.egg-info/dependency_links.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)       44 2023-11-02 07:53:47.000000 cloudlift-2.0.4/cloudlift.egg-info/entry_points.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)      384 2023-11-02 07:53:47.000000 cloudlift-2.0.4/cloudlift.egg-info/requires.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)       10 2023-11-02 07:53:47.000000 cloudlift-2.0.4/cloudlift.egg-info/top_level.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2020-01-19 03:14:24.000000 cloudlift-2.0.4/cloudlift.egg-info/zip-safe
--rw-r--r--   0 shoan     (1000) shoan     (1000)      100 2021-03-16 11:07:35.000000 cloudlift-2.0.4/pyproject.toml
--rw-r--r--   0 shoan     (1000) shoan     (1000)      383 2023-10-03 12:20:10.000000 cloudlift-2.0.4/requirements.txt
--rw-r--r--   0 shoan     (1000) shoan     (1000)       38 2023-11-02 07:53:49.435930 cloudlift-2.0.4/setup.cfg
--rw-r--r--   0 shoan     (1000) shoan     (1000)      774 2023-10-03 12:20:10.000000 cloudlift-2.0.4/setup.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-11-02 07:53:49.407116 cloudlift-2.0.4/test/
--rw-r--r--   0 shoan     (1000) shoan     (1000)     5303 2023-10-03 12:20:10.000000 cloudlift-2.0.4/test/test_cloudlift.py
--rwxrwxrwx   0 shoan     (1000) shoan     (1000)     2787 2023-08-13 02:51:34.000000 cloudlift-2.0.4/test/test_cloudlift_cluster.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.363932 cloudlift-2.0.5/
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1062 2020-04-14 13:38:03.000000 cloudlift-2.0.5/LICENSE
+-rwx------   0 shoan     (1000) shoan     (1000)       40 2020-02-21 06:48:18.000000 cloudlift-2.0.5/MANIFEST.in
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    13573 2024-04-15 15:46:14.360011 cloudlift-2.0.5/PKG-INFO
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    13309 2023-12-04 09:29:06.000000 cloudlift-2.0.5/README.md
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:13.543328 cloudlift-2.0.5/cloudlift/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6400 2023-04-26 12:53:28.000000 cloudlift-2.0.5/cloudlift/__init__.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:13.920612 cloudlift-2.0.5/cloudlift/config/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      266 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      669 2024-03-14 07:26:45.000000 cloudlift-2.0.5/cloudlift/config/account.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      448 2023-02-02 08:10:32.000000 cloudlift-2.0.5/cloudlift/config/banner.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      621 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/decimal_encoder.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     2408 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/diff.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1844 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/dynamodb_configuration.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    22093 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/config/environment_configuration.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      546 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/logging.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     2129 2024-04-15 12:48:19.000000 cloudlift-2.0.5/cloudlift/config/mfa.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     4387 2023-01-25 11:43:34.000000 cloudlift-2.0.5/cloudlift/config/parameter_store.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     2568 2023-04-26 12:53:28.000000 cloudlift-2.0.5/cloudlift/config/pre_flight.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     3516 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/region.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    20176 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/config/service_configuration.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      161 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/config/stack.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     7127 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/config/utils.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      217 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/constants.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.219932 cloudlift-2.0.5/cloudlift/deployment/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      373 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     3154 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/changesets.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    41735 2024-01-23 15:20:25.000000 cloudlift-2.0.5/cloudlift/deployment/cluster_template_generator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      267 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/configs.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6391 2023-07-18 05:11:33.000000 cloudlift-2.0.5/cloudlift/deployment/deployer.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     7658 2024-04-15 15:41:57.000000 cloudlift-2.0.5/cloudlift/deployment/ecr_client.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    18003 2024-04-15 12:48:19.000000 cloudlift-2.0.5/cloudlift/deployment/ecs.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      996 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/editor.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     8032 2023-12-04 18:19:19.000000 cloudlift-2.0.5/cloudlift/deployment/environment_creator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      896 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/progress.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6646 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/service_creator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     7056 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/deployment/service_information_fetcher.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    46514 2023-12-04 09:29:06.000000 cloudlift-2.0.5/cloudlift/deployment/service_template_generator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     4397 2023-02-02 08:10:32.000000 cloudlift-2.0.5/cloudlift/deployment/service_updater.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6527 2023-04-26 12:53:28.000000 cloudlift-2.0.5/cloudlift/deployment/task_definition_creator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1257 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/deployment/template_generator.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.253934 cloudlift-2.0.5/cloudlift/exceptions/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       46 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/exceptions/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      154 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/exceptions/exceptions.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.292934 cloudlift-2.0.5/cloudlift/session/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       30 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/session/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1874 2022-12-15 11:12:05.000000 cloudlift-2.0.5/cloudlift/session/session_creator.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.310968 cloudlift-2.0.5/cloudlift/version/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       18 2024-04-15 15:41:57.000000 cloudlift-2.0.5/cloudlift/version/__init__.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:13.643926 cloudlift-2.0.5/cloudlift.egg-info/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    13573 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/PKG-INFO
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1665 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)       44 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/entry_points.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)      384 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/requires.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)       10 2024-04-15 15:46:13.000000 cloudlift-2.0.5/cloudlift.egg-info/top_level.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2020-01-19 03:14:24.000000 cloudlift-2.0.5/cloudlift.egg-info/zip-safe
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      100 2021-03-16 11:07:35.000000 cloudlift-2.0.5/pyproject.toml
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      383 2024-04-15 12:48:19.000000 cloudlift-2.0.5/requirements.txt
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       38 2024-04-15 15:46:14.364932 cloudlift-2.0.5/setup.cfg
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      774 2023-12-04 09:29:06.000000 cloudlift-2.0.5/setup.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2024-04-15 15:46:14.340963 cloudlift-2.0.5/test/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     5303 2023-12-04 09:29:06.000000 cloudlift-2.0.5/test/test_cloudlift.py
+-rwx------   0 shoan     (1000) shoan     (1000)     2787 2023-08-13 02:51:34.000000 cloudlift-2.0.5/test/test_cloudlift_cluster.py
```

### Comparing `cloudlift-2.0.4/LICENSE` & `cloudlift-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/PKG-INFO` & `cloudlift-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlift
-Version: 2.0.4
+Version: 2.0.5
 Summary: Cloudlift makes it easier to launch dockerized services in AWS ECS
 Home-page: https://github.com/GetSimpl/cloudlift
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cloudlift
```

### Comparing `cloudlift-2.0.4/README.md` & `cloudlift-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/__init__.py` & `cloudlift-2.0.5/cloudlift/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/account.py` & `cloudlift-2.0.5/cloudlift/config/account.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/decimal_encoder.py` & `cloudlift-2.0.5/cloudlift/config/decimal_encoder.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/diff.py` & `cloudlift-2.0.5/cloudlift/config/diff.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/dynamodb_configuration.py` & `cloudlift-2.0.5/cloudlift/config/dynamodb_configuration.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/environment_configuration.py` & `cloudlift-2.0.5/cloudlift/config/environment_configuration.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/logging.py` & `cloudlift-2.0.5/cloudlift/config/logging.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/mfa.py` & `cloudlift-2.0.5/cloudlift/config/mfa.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/parameter_store.py` & `cloudlift-2.0.5/cloudlift/config/parameter_store.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/pre_flight.py` & `cloudlift-2.0.5/cloudlift/config/pre_flight.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/region.py` & `cloudlift-2.0.5/cloudlift/config/region.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/service_configuration.py` & `cloudlift-2.0.5/cloudlift/config/service_configuration.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/config/utils.py` & `cloudlift-2.0.5/cloudlift/config/utils.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/changesets.py` & `cloudlift-2.0.5/cloudlift/deployment/changesets.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/cluster_template_generator.py` & `cloudlift-2.0.5/cloudlift/deployment/cluster_template_generator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/deployer.py` & `cloudlift-2.0.5/cloudlift/deployment/deployer.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/ecr_client.py` & `cloudlift-2.0.5/cloudlift/deployment/ecr_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,34 @@
 from stringcase import spinalcase
 
 
 from cloudlift.config import get_account_id
 from cloudlift.config.logging import log_intent, log_warning, log_bold, log_err
 
 
+def get_container_tool() -> str:
+    """
+    Detect whether docker or podman is available. Use podman or fall back to docker
+    """
+    from shutil import which
+    tool = which ('podman') or which('docker')
+    if tool is None:
+        raise UnrecoverableException('Podman not installed')
+    log_intent(f"Using {tool} as container tool")
+    return tool
+
+
 class EcrClient:
     def __init__(self, name, region, build_args=None, working_dir='.'):
         self.name = name
         self.build_args = build_args
         self.working_dir = working_dir
         self.region = region
         self.ecr_client = boto3.session.Session(region_name=self.region).client('ecr')
+        self.container_tool = get_container_tool()
 
     def build_and_upload_image(self):
         self._ensure_repository()
         self._ensure_image_in_ecr()
 
     def upload_image(self, version, additional_tags):
         image_name = spinalcase(self.name) + ':' + version
@@ -94,38 +107,38 @@
         version to be " + self.version + " based on current status")
             else:
                 self.version = self._find_commit_sha()
                 log_intent("Version parameter was not provided. Determined \
         version to be " + self.version + " based on current status")
 
     def _build_image(self, image_name):
-        log_bold("Building docker image " + image_name)
+        log_bold("Building container image " + image_name)
         command = self._build_command(image_name)
         subprocess.check_call(command, shell=True)
         log_bold("Built " + image_name)
 
     def _build_command(self, image_name):
         if self.build_args is None:
-            return f'docker build -t {image_name} {self.working_dir}'
+            return f'{self.container_tool} build -t {image_name} {self.working_dir}'
         else:
             build_args_command_fragment = []
             for k, v in self.build_args.items():
                 build_args_command_fragment.append(" --build-arg " + "=".join((k, v)))
-            return f'docker build -t {image_name}{"".join(build_args_command_fragment)} {self.working_dir}'
+            return f'{self.container_tool} build -t {image_name}{"".join(build_args_command_fragment)} {self.working_dir}'
 
     def _login_to_ecr(self):
         log_intent("Attempting login...")
         auth_token_res = self.ecr_client.get_authorization_token()
         user, auth_token = base64.b64decode(
             auth_token_res['authorizationData'][0]['authorizationToken']
         ).decode("utf-8").split(':')
-        ecr_url = auth_token_res['authorizationData'][0]['proxyEndpoint']
-        subprocess.check_call(["docker", "login", "-u", user,
+        ecr_url = auth_token_res['authorizationData'][0]['proxyEndpoint'].removeprefix("https://")
+        subprocess.check_call([self.container_tool, "login", "-u", user,
                                "-p", auth_token, ecr_url])
-        log_intent('Docker login to ECR succeeded.')
+        log_intent(f'{self.container_tool_name} login to ECR succeeded.')
 
     def _find_commit_sha(self, version=None):
         log_intent("Finding commit SHA")
         try:
             version_to_find = version or "HEAD"
             commit_sha = subprocess.check_output(
                 ["git", "rev-list", "-n", "1", version_to_find]
@@ -134,20 +147,20 @@
             return commit_sha
         except:
             raise UnrecoverableException("Commit SHA not found. Given version is not a git tag, \
 branch or commit SHA")
 
     def _push_image(self, local_name, ecr_name):
         try:
-            subprocess.check_call(["docker", "tag", local_name, ecr_name])
+            subprocess.check_call([self.container_tool, "tag", local_name, ecr_name])
         except:
             raise UnrecoverableException("Local image was not found.")
         self._login_to_ecr()
-        subprocess.check_call(["docker", "push", ecr_name])
-        subprocess.check_call(["docker", "rmi", ecr_name])
+        subprocess.check_call([self.container_tool, "push", ecr_name])
+        subprocess.check_call([self.container_tool, "rmi", ecr_name])
         log_intent('Pushed the image (' + local_name + ') to ECR sucessfully.')
 
     def _add_image_tag(self, existing_tag, new_tag):
         try:
             image_manifest = self.ecr_client.batch_get_image(
                 repositoryName=self.repo_name,
                 imageIds=[
@@ -178,7 +191,10 @@
     def ecr_image_uri(self):
         return str(self.account_id) + ".dkr.ecr." + self.region + \
                ".amazonaws.com/" + self.repo_name
 
     @property
     def account_id(self):
         return get_account_id()
+    @property
+    def container_tool_name(self):
+        return self.container_tool.split('/')[-1] if self.container_tool is not None else None
```

### Comparing `cloudlift-2.0.4/cloudlift/deployment/ecs.py` & `cloudlift-2.0.5/cloudlift/deployment/ecs.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/editor.py` & `cloudlift-2.0.5/cloudlift/deployment/editor.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/environment_creator.py` & `cloudlift-2.0.5/cloudlift/deployment/environment_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/progress.py` & `cloudlift-2.0.5/cloudlift/deployment/progress.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/service_creator.py` & `cloudlift-2.0.5/cloudlift/deployment/service_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/service_information_fetcher.py` & `cloudlift-2.0.5/cloudlift/deployment/service_information_fetcher.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/service_template_generator.py` & `cloudlift-2.0.5/cloudlift/deployment/service_template_generator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/service_updater.py` & `cloudlift-2.0.5/cloudlift/deployment/service_updater.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/task_definition_creator.py` & `cloudlift-2.0.5/cloudlift/deployment/task_definition_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/deployment/template_generator.py` & `cloudlift-2.0.5/cloudlift/deployment/template_generator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift/session/session_creator.py` & `cloudlift-2.0.5/cloudlift/session/session_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/cloudlift.egg-info/PKG-INFO` & `cloudlift-2.0.5/cloudlift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlift
-Version: 2.0.4
+Version: 2.0.5
 Summary: Cloudlift makes it easier to launch dockerized services in AWS ECS
 Home-page: https://github.com/GetSimpl/cloudlift
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cloudlift
```

### Comparing `cloudlift-2.0.4/cloudlift.egg-info/SOURCES.txt` & `cloudlift-2.0.5/cloudlift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/setup.py` & `cloudlift-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/test/test_cloudlift.py` & `cloudlift-2.0.5/test/test_cloudlift.py`

 * *Files identical despite different names*

### Comparing `cloudlift-2.0.4/test/test_cloudlift_cluster.py` & `cloudlift-2.0.5/test/test_cloudlift_cluster.py`

 * *Files identical despite different names*

