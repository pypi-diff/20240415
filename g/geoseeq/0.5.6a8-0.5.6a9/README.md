# Comparing `tmp/geoseeq-0.5.6a8.tar.gz` & `tmp/geoseeq-0.5.6a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoseeq-0.5.6a8.tar", last modified: Fri Apr  5 16:51:54 2024, max compression
+gzip compressed data, was "geoseeq-0.5.6a9.tar", last modified: Fri Apr  5 17:19:16 2024, max compression
```

## Comparing `geoseeq-0.5.6a8.tar` & `geoseeq-0.5.6a9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.583830 geoseeq-0.5.6a8/
--rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.5.6a8/LICENSE
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-05 16:51:54.583407 geoseeq-0.5.6a8/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     4254 2023-10-24 18:48:30.000000 geoseeq-0.5.6a8/README.md
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.552427 geoseeq-0.5.6a8/geoseeq/
--rw-r--r--   0 dcdanko    (501) staff       (20)      946 2024-03-19 13:54:16.000000 geoseeq-0.5.6a8/geoseeq/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-08-14 20:18:48.000000 geoseeq-0.5.6a8/geoseeq/app.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      188 2023-08-25 17:37:47.000000 geoseeq-0.5.6a8/geoseeq/blob_constructors.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-07-05 19:40:08.000000 geoseeq-0.5.6a8/geoseeq/bulk_creators.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.560518 geoseeq-0.5.6a8/geoseeq/cli/
--rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/cli/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/cli/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2275 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/copy.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4132 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/detail.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    17656 2024-03-19 02:18:54.000000 geoseeq-0.5.6a8/geoseeq/cli/download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2024-01-08 16:45:41.000000 geoseeq-0.5.6a8/geoseeq/cli/fastq_utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      997 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/get_eula.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3259 2024-04-05 16:51:46.000000 geoseeq-0.5.6a8/geoseeq/cli/main.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5929 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/manage.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      738 2023-08-22 16:00:03.000000 geoseeq-0.5.6a8/geoseeq/cli/progress_bar.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3838 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/run.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1015 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/search.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.563403 geoseeq-0.5.6a8/geoseeq/cli/shared_params/
--rw-r--r--   0 dcdanko    (501) staff       (20)      325 2024-03-19 02:06:03.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4095 2024-03-21 02:47:29.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/common_state.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1072 2024-03-14 13:34:44.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/config.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9299 2024-03-19 02:05:53.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/id_handlers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2741 2023-08-22 14:05:04.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/obj_getters.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1948 2024-03-19 02:15:47.000000 geoseeq-0.5.6a8/geoseeq/cli/shared_params/opts_and_args.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.565222 geoseeq-0.5.6a8/geoseeq/cli/upload/
--rw-r--r--   0 dcdanko    (501) staff       (20)      627 2024-03-18 18:33:30.000000 geoseeq-0.5.6a8/geoseeq/cli/upload/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9035 2024-04-05 16:48:06.000000 geoseeq-0.5.6a8/geoseeq/cli/upload/upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3434 2023-11-09 22:36:49.000000 geoseeq-0.5.6a8/geoseeq/cli/upload/upload_advanced.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7303 2024-04-05 16:48:16.000000 geoseeq-0.5.6a8/geoseeq/cli/upload/upload_reads.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.5.6a8/geoseeq/cli/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2873 2023-08-10 17:50:03.000000 geoseeq-0.5.6a8/geoseeq/cli/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6783 2024-02-05 19:19:37.000000 geoseeq-0.5.6a8/geoseeq/cli/view.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      431 2024-02-26 20:12:47.000000 geoseeq-0.5.6a8/geoseeq/constants.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.565802 geoseeq-0.5.6a8/geoseeq/contrib/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/contrib/__init__.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.567462 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/api.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/bioproject.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/contrib/ncbi/setup_logging.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4138 2024-04-05 15:21:33.000000 geoseeq-0.5.6a8/geoseeq/file_system_cache.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.571229 geoseeq-0.5.6a8/geoseeq/id_constructors/
--rw-r--r--   0 dcdanko    (501) staff       (20)      126 2023-08-25 17:28:11.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5702 2024-03-21 02:39:35.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/from_blobs.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3151 2024-04-01 15:41:03.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/from_ids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4174 2024-02-26 20:07:19.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/from_names.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3305 2024-02-26 20:08:43.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/from_uuids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2676 2024-02-26 20:08:58.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/resolvers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      723 2023-08-25 17:06:17.000000 geoseeq-0.5.6a8/geoseeq/id_constructors/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7898 2024-02-26 20:25:43.000000 geoseeq-0.5.6a8/geoseeq/knex.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-07-05 19:40:08.000000 geoseeq-0.5.6a8/geoseeq/organization.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9873 2023-11-19 15:30:12.000000 geoseeq-0.5.6a8/geoseeq/pipeline.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.573017 geoseeq-0.5.6a8/geoseeq/plotting/
--rw-r--r--   0 dcdanko    (501) staff       (20)      154 2023-08-25 16:47:04.000000 geoseeq-0.5.6a8/geoseeq/plotting/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      285 2023-08-23 12:02:35.000000 geoseeq-0.5.6a8/geoseeq/plotting/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4096 2023-08-23 13:09:29.000000 geoseeq-0.5.6a8/geoseeq/plotting/highcharts.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.574543 geoseeq-0.5.6a8/geoseeq/plotting/map/
--rw-r--r--   0 dcdanko    (501) staff       (20)      295 2023-10-24 03:32:07.000000 geoseeq-0.5.6a8/geoseeq/plotting/map/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4329 2023-10-24 03:21:34.000000 geoseeq-0.5.6a8/geoseeq/plotting/map/base_layer.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3907 2023-10-24 13:01:18.000000 geoseeq-0.5.6a8/geoseeq/plotting/map/map.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1795 2023-10-24 03:17:14.000000 geoseeq-0.5.6a8/geoseeq/plotting/map/overlay.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2554 2023-08-25 17:58:17.000000 geoseeq-0.5.6a8/geoseeq/plotting/selectable.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    13741 2024-03-19 02:51:49.000000 geoseeq-0.5.6a8/geoseeq/project.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7131 2024-04-02 19:52:31.000000 geoseeq-0.5.6a8/geoseeq/remote_object.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.577933 geoseeq-0.5.6a8/geoseeq/result/
--rw-r--r--   0 dcdanko    (501) staff       (20)      356 2023-08-10 17:50:03.000000 geoseeq-0.5.6a8/geoseeq/result/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1782 2023-08-10 17:50:03.000000 geoseeq-0.5.6a8/geoseeq/result/bioinfo.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5568 2024-04-02 20:04:55.000000 geoseeq-0.5.6a8/geoseeq/result/file_download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    11496 2024-04-05 16:47:18.000000 geoseeq-0.5.6a8/geoseeq/result/file_upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8433 2024-03-19 02:18:12.000000 geoseeq-0.5.6a8/geoseeq/result/result_file.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    11122 2024-03-18 21:38:47.000000 geoseeq-0.5.6a8/geoseeq/result/result_folder.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2772 2023-08-13 00:53:07.000000 geoseeq-0.5.6a8/geoseeq/result/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7981 2024-03-19 02:10:10.000000 geoseeq-0.5.6a8/geoseeq/sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3388 2023-10-05 16:43:42.000000 geoseeq-0.5.6a8/geoseeq/search.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7206 2024-04-05 16:46:50.000000 geoseeq-0.5.6a8/geoseeq/upload_download_manager.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3577 2024-02-26 20:12:33.000000 geoseeq-0.5.6a8/geoseeq/utils.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.581246 geoseeq-0.5.6a8/geoseeq/vc/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.5.6a8/geoseeq/vc/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.5.6a8/geoseeq/vc/checksum.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2803 2023-08-25 17:39:54.000000 geoseeq-0.5.6a8/geoseeq/vc/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/vc/clone.py
--rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/vc/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/vc/vc_cache.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.5.6a8/geoseeq/vc/vc_dir.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3850 2023-08-25 17:41:01.000000 geoseeq-0.5.6a8/geoseeq/vc/vc_sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3110 2023-08-25 17:40:12.000000 geoseeq-0.5.6a8/geoseeq/vc/vc_stub.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-07-05 19:40:08.000000 geoseeq-0.5.6a8/geoseeq/work_orders.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.582995 geoseeq-0.5.6a8/geoseeq.egg-info/
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     2441 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/SOURCES.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)        1 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/dependency_links.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       45 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/entry_points.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       14 2024-04-05 16:51:54.000000 geoseeq-0.5.6a8/geoseeq.egg-info/top_level.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)      643 2024-04-05 16:51:38.000000 geoseeq-0.5.6a8/pyproject.toml
--rw-r--r--   0 dcdanko    (501) staff       (20)       38 2024-04-05 16:51:54.583901 geoseeq-0.5.6a8/setup.cfg
--rw-r--r--   0 dcdanko    (501) staff       (20)      801 2024-04-02 20:05:00.000000 geoseeq-0.5.6a8/setup.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 16:51:54.582338 geoseeq-0.5.6a8/tests/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.5.6a8/tests/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    12810 2023-10-24 13:59:25.000000 geoseeq-0.5.6a8/tests/test_api_client.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      784 2023-10-24 13:03:13.000000 geoseeq-0.5.6a8/tests/test_plotting.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.681753 geoseeq-0.5.6a9/
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.5.6a9/LICENSE
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-05 17:19:16.681468 geoseeq-0.5.6a9/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4254 2023-10-24 18:48:30.000000 geoseeq-0.5.6a9/README.md
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.659236 geoseeq-0.5.6a9/geoseeq/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      946 2024-03-19 13:54:16.000000 geoseeq-0.5.6a9/geoseeq/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-08-14 20:18:48.000000 geoseeq-0.5.6a9/geoseeq/app.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      188 2023-08-25 17:37:47.000000 geoseeq-0.5.6a9/geoseeq/blob_constructors.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-07-05 19:40:08.000000 geoseeq-0.5.6a9/geoseeq/bulk_creators.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.663925 geoseeq-0.5.6a9/geoseeq/cli/
+-rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/cli/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/cli/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2275 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/copy.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4132 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/detail.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    17656 2024-03-19 02:18:54.000000 geoseeq-0.5.6a9/geoseeq/cli/download.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2024-01-08 16:45:41.000000 geoseeq-0.5.6a9/geoseeq/cli/fastq_utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      997 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/get_eula.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3259 2024-04-05 17:18:22.000000 geoseeq-0.5.6a9/geoseeq/cli/main.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5929 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/manage.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      738 2023-08-22 16:00:03.000000 geoseeq-0.5.6a9/geoseeq/cli/progress_bar.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3838 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/run.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1015 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/search.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.666206 geoseeq-0.5.6a9/geoseeq/cli/shared_params/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      325 2024-03-19 02:06:03.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4095 2024-03-21 02:47:29.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/common_state.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1072 2024-03-14 13:34:44.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/config.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9299 2024-03-19 02:05:53.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/id_handlers.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2741 2023-08-22 14:05:04.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/obj_getters.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2083 2024-04-05 17:01:58.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/opts_and_args.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.667732 geoseeq-0.5.6a9/geoseeq/cli/upload/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      627 2024-03-18 18:33:30.000000 geoseeq-0.5.6a9/geoseeq/cli/upload/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9203 2024-04-05 17:16:22.000000 geoseeq-0.5.6a9/geoseeq/cli/upload/upload.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3434 2023-11-09 22:36:49.000000 geoseeq-0.5.6a9/geoseeq/cli/upload/upload_advanced.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7450 2024-04-05 17:17:32.000000 geoseeq-0.5.6a9/geoseeq/cli/upload/upload_reads.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.5.6a9/geoseeq/cli/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2873 2023-08-10 17:50:03.000000 geoseeq-0.5.6a9/geoseeq/cli/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     6783 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/view.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      431 2024-02-26 20:12:47.000000 geoseeq-0.5.6a9/geoseeq/constants.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.668064 geoseeq-0.5.6a9/geoseeq/contrib/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/contrib/__init__.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.669219 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/api.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/bioproject.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/setup_logging.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4138 2024-04-05 15:21:33.000000 geoseeq-0.5.6a9/geoseeq/file_system_cache.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.671175 geoseeq-0.5.6a9/geoseeq/id_constructors/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      126 2023-08-25 17:28:11.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5702 2024-03-21 02:39:35.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/from_blobs.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3151 2024-04-01 15:41:03.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/from_ids.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4174 2024-02-26 20:07:19.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/from_names.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3305 2024-02-26 20:08:43.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/from_uuids.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2676 2024-02-26 20:08:58.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/resolvers.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      723 2023-08-25 17:06:17.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7898 2024-02-26 20:25:43.000000 geoseeq-0.5.6a9/geoseeq/knex.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-07-05 19:40:08.000000 geoseeq-0.5.6a9/geoseeq/organization.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     9873 2023-11-19 15:30:12.000000 geoseeq-0.5.6a9/geoseeq/pipeline.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.672288 geoseeq-0.5.6a9/geoseeq/plotting/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      154 2023-08-25 16:47:04.000000 geoseeq-0.5.6a9/geoseeq/plotting/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      285 2023-08-23 12:02:35.000000 geoseeq-0.5.6a9/geoseeq/plotting/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4096 2023-08-23 13:09:29.000000 geoseeq-0.5.6a9/geoseeq/plotting/highcharts.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.673343 geoseeq-0.5.6a9/geoseeq/plotting/map/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      295 2023-10-24 03:32:07.000000 geoseeq-0.5.6a9/geoseeq/plotting/map/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4329 2023-10-24 03:21:34.000000 geoseeq-0.5.6a9/geoseeq/plotting/map/base_layer.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3907 2023-10-24 13:01:18.000000 geoseeq-0.5.6a9/geoseeq/plotting/map/map.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1795 2023-10-24 03:17:14.000000 geoseeq-0.5.6a9/geoseeq/plotting/map/overlay.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2554 2023-08-25 17:58:17.000000 geoseeq-0.5.6a9/geoseeq/plotting/selectable.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    13741 2024-03-19 02:51:49.000000 geoseeq-0.5.6a9/geoseeq/project.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7131 2024-04-02 19:52:31.000000 geoseeq-0.5.6a9/geoseeq/remote_object.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.675781 geoseeq-0.5.6a9/geoseeq/result/
+-rw-r--r--   0 dcdanko    (501) staff       (20)      356 2023-08-10 17:50:03.000000 geoseeq-0.5.6a9/geoseeq/result/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     1782 2023-08-10 17:50:03.000000 geoseeq-0.5.6a9/geoseeq/result/bioinfo.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     5568 2024-04-02 20:04:55.000000 geoseeq-0.5.6a9/geoseeq/result/file_download.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    11696 2024-04-05 17:15:32.000000 geoseeq-0.5.6a9/geoseeq/result/file_upload.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8677 2024-04-05 17:13:21.000000 geoseeq-0.5.6a9/geoseeq/result/result_file.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    11122 2024-03-18 21:38:47.000000 geoseeq-0.5.6a9/geoseeq/result/result_folder.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2772 2023-08-13 00:53:07.000000 geoseeq-0.5.6a9/geoseeq/result/utils.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7981 2024-03-19 02:10:10.000000 geoseeq-0.5.6a9/geoseeq/sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3388 2023-10-05 16:43:42.000000 geoseeq-0.5.6a9/geoseeq/search.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     7423 2024-04-05 17:09:10.000000 geoseeq-0.5.6a9/geoseeq/upload_download_manager.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/user.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3577 2024-02-26 20:12:33.000000 geoseeq-0.5.6a9/geoseeq/utils.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.679529 geoseeq-0.5.6a9/geoseeq/vc/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.5.6a9/geoseeq/vc/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.5.6a9/geoseeq/vc/checksum.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2803 2023-08-25 17:39:54.000000 geoseeq-0.5.6a9/geoseeq/vc/cli.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/vc/clone.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/vc/constants.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/vc/vc_cache.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/vc/vc_dir.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3850 2023-08-25 17:41:01.000000 geoseeq-0.5.6a9/geoseeq/vc/vc_sample.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     3110 2023-08-25 17:40:12.000000 geoseeq-0.5.6a9/geoseeq/vc/vc_stub.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-07-05 19:40:08.000000 geoseeq-0.5.6a9/geoseeq/work_orders.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.681161 geoseeq-0.5.6a9/geoseeq.egg-info/
+-rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/PKG-INFO
+-rw-r--r--   0 dcdanko    (501) staff       (20)     2441 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/SOURCES.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)        1 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/dependency_links.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       45 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/entry_points.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)       14 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/top_level.txt
+-rw-r--r--   0 dcdanko    (501) staff       (20)      643 2024-04-05 17:18:45.000000 geoseeq-0.5.6a9/pyproject.toml
+-rw-r--r--   0 dcdanko    (501) staff       (20)       38 2024-04-05 17:19:16.681809 geoseeq-0.5.6a9/setup.cfg
+-rw-r--r--   0 dcdanko    (501) staff       (20)      831 2024-04-05 17:19:10.000000 geoseeq-0.5.6a9/setup.py
+drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.680379 geoseeq-0.5.6a9/tests/
+-rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.5.6a9/tests/__init__.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)    12810 2023-10-24 13:59:25.000000 geoseeq-0.5.6a9/tests/test_api_client.py
+-rw-r--r--   0 dcdanko    (501) staff       (20)      784 2023-10-24 13:03:13.000000 geoseeq-0.5.6a9/tests/test_plotting.py
```

### Comparing `geoseeq-0.5.6a8/LICENSE` & `geoseeq-0.5.6a9/LICENSE`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/PKG-INFO` & `geoseeq-0.5.6a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a8
+Version: 0.5.6a9
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a8/README.md` & `geoseeq-0.5.6a9/README.md`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/__init__.py` & `geoseeq-0.5.6a9/geoseeq/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/app.py` & `geoseeq-0.5.6a9/geoseeq/app.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/bulk_creators.py` & `geoseeq-0.5.6a9/geoseeq/bulk_creators.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/copy.py` & `geoseeq-0.5.6a9/geoseeq/cli/copy.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/detail.py` & `geoseeq-0.5.6a9/geoseeq/cli/detail.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/download.py` & `geoseeq-0.5.6a9/geoseeq/cli/download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/fastq_utils.py` & `geoseeq-0.5.6a9/geoseeq/cli/fastq_utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/get_eula.py` & `geoseeq-0.5.6a9/geoseeq/cli/get_eula.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/main.py` & `geoseeq-0.5.6a9/geoseeq/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """Print the version of the Geoseeq API being used.
 
     ---
     
     Use of this tool implies acceptance of the GeoSeeq End User License Agreement.
     Run `geoseeq eula show` to view the EULA.
     """
-    click.echo('0.5.6a8')  # remember to update setup
+    click.echo('0.5.6a9')  # remember to update setup
 
 
 @main.group('advanced')
 def cli_advanced():
     """Advanced commands."""
     pass
```

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/manage.py` & `geoseeq-0.5.6a9/geoseeq/cli/manage.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/progress_bar.py` & `geoseeq-0.5.6a9/geoseeq/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/run.py` & `geoseeq-0.5.6a9/geoseeq/cli/run.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/search.py` & `geoseeq-0.5.6a9/geoseeq/cli/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/shared_params/common_state.py` & `geoseeq-0.5.6a9/geoseeq/cli/shared_params/common_state.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/shared_params/config.py` & `geoseeq-0.5.6a9/geoseeq/cli/shared_params/config.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/shared_params/id_handlers.py` & `geoseeq-0.5.6a9/geoseeq/cli/shared_params/id_handlers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/shared_params/obj_getters.py` & `geoseeq-0.5.6a9/geoseeq/cli/shared_params/obj_getters.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/shared_params/opts_and_args.py` & `geoseeq-0.5.6a9/geoseeq/cli/shared_params/opts_and_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 
 dryrun_option = click.option('--dryrun/--wetrun', default=False, help='Print what will be created without actually creating it')
 overwrite_option = click.option('--overwrite/--no-overwrite', default=False, help='Overwrite existing samples, files, and data')
-
+no_new_versions_option = click.option('--no-new-versions/--new-versions', default=False, help='Do not create new versions of the data')
 def module_option(options, use_default=True, default=None):
     if use_default:
         default = default or options[0]
     if default and not use_default:
         raise ValueError('Cannot specify a default value without use_default=True')
     return click.option('-m', '--module-name', type=click.Choice(options), default=default, help='Name for the module that will store the data')
```

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/upload/__init__.py` & `geoseeq-0.5.6a9/geoseeq/cli/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/upload/upload.py` & `geoseeq-0.5.6a9/geoseeq/cli/upload/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     folder_id_arg,
     handle_folder_id,
     overwrite_option,
     project_id_arg,
     handle_project_id,
     project_or_sample_id_arg,
     handle_project_or_sample_id,
+    no_new_versions_option,
 )
 from geoseeq.upload_download_manager import GeoSeeqUploadManager
 
 logger = logging.getLogger('geoseeq_api')
 
 recursive_option = click.option('--recursive/--no-recursive', default=True, help='Upload files in subfolders')
 hidden_option = click.option('--hidden/--no-hidden', default=False, help='Upload hidden files in subfolders')
@@ -37,19 +38,20 @@
 @use_common_state
 @click.option('--cores', default=1, help='Number of uploads to run in parallel')
 @yes_option
 @private_option
 @link_option
 @recursive_option
 @hidden_option
+@no_new_versions_option
 @click.option('-n', '--geoseeq-file-name', default=None, multiple=True,
               help='Specify a different name for the file on GeoSeeq than the local file name.')
 @folder_id_arg
 @click.argument('file_paths', type=click.Path(exists=True), nargs=-1)
-def cli_upload_file(state, cores, yes, private, link_type, recursive, hidden, geoseeq_file_name, folder_id, file_paths):
+def cli_upload_file(state, cores, yes, private, link_type, recursive, hidden, no_new_versions, geoseeq_file_name, folder_id, file_paths):
     """Upload files to GeoSeeq.
 
     This command uploads files to either a sample or project on GeoSeeq. It can be used to upload
     multiple files to the same folder at once.
     
     ---
 
@@ -103,15 +105,15 @@
         name_pairs = zip([basename(fp) for fp in file_paths], file_paths)
     
     upload_manager = GeoSeeqUploadManager(
         n_parallel_uploads=cores,
         link_type=link_type,
         progress_tracker_factory=PBarManager().get_new_bar,
         log_level=state.log_level,
-        overwrite=True,
+        no_new_versions=no_new_versions,
         use_cache=state.use_cache,
     )
     for geoseeq_file_name, file_path in name_pairs:
         if isfile(file_path):
             upload_manager.add_local_file_to_result_folder(result_folder, file_path)
         elif isdir(file_path) and recursive:
             upload_manager.add_local_folder_to_result_folder(result_folder, file_path, recursive=recursive, hidden_files=hidden, prefix=file_path)
@@ -127,26 +129,28 @@
 @click.command('folders')
 @use_common_state
 @click.option('--cores', default=1, help='Number of uploads to run in parallel')
 @yes_option
 @private_option
 @recursive_option
 @hidden_option
+@no_new_versions_option
 @project_or_sample_id_arg
 @click.argument('folder_names', type=click.Path(exists=True), nargs=-1)
-def cli_upload_folder(state, cores, yes, private, recursive, hidden, project_or_sample_id, folder_names):
+def cli_upload_folder(state, cores, yes, private, recursive, hidden, no_new_versions, project_or_sample_id, folder_names):
     knex = state.get_knex()
     root_obj = handle_project_or_sample_id(knex, project_or_sample_id, yes=yes, private=private)
     upload_manager = GeoSeeqUploadManager(
         n_parallel_uploads=cores,
         link_type='upload',
         progress_tracker_factory=PBarManager().get_new_bar,
         log_level=logging.INFO,
         overwrite=True,
         use_cache=state.use_cache,
+        no_new_versions=no_new_versions,
     )
     for folder_name in folder_names:
         result_folder = root_obj.result_folder(folder_name).idem()
         upload_manager.add_local_folder_to_result_folder(result_folder, folder_name, recursive=recursive, hidden_files=hidden)
     click.echo(upload_manager.get_preview_string(), err=True)
     if not yes:
         click.confirm('Continue?', abort=True)
```

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/upload/upload_advanced.py` & `geoseeq-0.5.6a9/geoseeq/cli/upload/upload_advanced.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/upload/upload_reads.py` & `geoseeq-0.5.6a9/geoseeq/cli/upload/upload_reads.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     private_option,
     link_option,
     module_option,
     project_id_arg,
     overwrite_option,
     yes_option,
     use_common_state,
+    no_new_versions_option
 )
 from geoseeq.upload_download_manager import GeoSeeqUploadManager
 
 from geoseeq.constants import FASTQ_MODULE_NAMES
 from geoseeq.cli.progress_bar import PBarManager
 
 logger = logging.getLogger('geoseeq_api')
@@ -81,25 +82,26 @@
             path = filepaths[filename]
             click.echo(f'    {seq_length}::{field_name}: {path}', err=True)
     if not yes:
         click.confirm('Do you want to upload these files?', abort=True)
     return groups
 
 
-def _do_upload(groups, module_name, link_type, lib, filepaths, overwrite, cores, state):
+def _do_upload(groups, module_name, link_type, lib, filepaths, overwrite, no_new_versions, cores, state):
 
     with requests.Session() as session:
         upload_manager = GeoSeeqUploadManager(
             n_parallel_uploads=cores,
             session=session,
             link_type=link_type,
             log_level=state.log_level,
             overwrite=overwrite,
             progress_tracker_factory=PBarManager().get_new_bar,
             use_cache=state.use_cache,
+            no_new_versions=no_new_versions,
         )
         for group in groups:
             sample = lib.sample(group['sample_name']).idem()
             read_folder = sample.result_folder(module_name).idem()
             for field_name, path in group['fields'].items():
                 result_file = read_folder.read_file(field_name)
                 upload_manager.add_result_file(result_file, filepaths[path])
@@ -135,18 +137,19 @@
 @use_common_state
 @click.option('--cores', default=1, help='Number of uploads to run in parallel')
 @overwrite_option
 @yes_option
 @click.option('--regex', default=None, help='An optional regex to use to extract sample names from the file names')
 @private_option
 @link_option
+@no_new_versions_option
 @module_option(FASTQ_MODULE_NAMES)
 @project_id_arg
 @click.argument('fastq_files', type=click.Path(exists=True), nargs=-1)
-def cli_upload_reads_wizard(state, cores, overwrite, yes, regex, private, link_type, module_name, project_id, fastq_files):
+def cli_upload_reads_wizard(state, cores, overwrite, yes, regex, private, link_type, no_new_versions, module_name, project_id, fastq_files):
     """Upload fastq read files to GeoSeeq.
 
     This command automatically groups files by their sample name, lane number
     and read number. It asks for confirmation before creating any samples or
     data.
 
     ---
@@ -192,8 +195,8 @@
     """
     knex = state.get_knex()
     proj = handle_project_id(knex, project_id, yes, private)
     filepaths = {basename(line): line for line in flatten_list_of_fastqs(fastq_files)}
     click.echo(f'Found {len(filepaths)} files to upload.', err=True)
     regex = _get_regex(knex, filepaths, module_name, proj, regex)
     groups = _group_files(knex, filepaths, module_name, regex, yes)
-    _do_upload(groups, module_name, link_type, proj, filepaths, overwrite, cores, state)
+    _do_upload(groups, module_name, link_type, proj, filepaths, overwrite, no_new_versions, cores, state)
```

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/user.py` & `geoseeq-0.5.6a9/geoseeq/cli/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/utils.py` & `geoseeq-0.5.6a9/geoseeq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/cli/view.py` & `geoseeq-0.5.6a9/geoseeq/cli/view.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/contrib/ncbi/api.py` & `geoseeq-0.5.6a9/geoseeq/contrib/ncbi/api.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/contrib/ncbi/bioproject.py` & `geoseeq-0.5.6a9/geoseeq/contrib/ncbi/bioproject.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/contrib/ncbi/cli.py` & `geoseeq-0.5.6a9/geoseeq/contrib/ncbi/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/file_system_cache.py` & `geoseeq-0.5.6a9/geoseeq/file_system_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/id_constructors/from_blobs.py` & `geoseeq-0.5.6a9/geoseeq/id_constructors/from_blobs.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/id_constructors/from_ids.py` & `geoseeq-0.5.6a9/geoseeq/id_constructors/from_ids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/id_constructors/from_names.py` & `geoseeq-0.5.6a9/geoseeq/id_constructors/from_names.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/id_constructors/from_uuids.py` & `geoseeq-0.5.6a9/geoseeq/id_constructors/from_uuids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/id_constructors/resolvers.py` & `geoseeq-0.5.6a9/geoseeq/id_constructors/resolvers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/id_constructors/utils.py` & `geoseeq-0.5.6a9/geoseeq/id_constructors/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/knex.py` & `geoseeq-0.5.6a9/geoseeq/knex.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/organization.py` & `geoseeq-0.5.6a9/geoseeq/organization.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/pipeline.py` & `geoseeq-0.5.6a9/geoseeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/plotting/highcharts.py` & `geoseeq-0.5.6a9/geoseeq/plotting/highcharts.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/plotting/map/base_layer.py` & `geoseeq-0.5.6a9/geoseeq/plotting/map/base_layer.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/plotting/map/map.py` & `geoseeq-0.5.6a9/geoseeq/plotting/map/map.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/plotting/map/overlay.py` & `geoseeq-0.5.6a9/geoseeq/plotting/map/overlay.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/plotting/selectable.py` & `geoseeq-0.5.6a9/geoseeq/plotting/selectable.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/project.py` & `geoseeq-0.5.6a9/geoseeq/project.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/remote_object.py` & `geoseeq-0.5.6a9/geoseeq/remote_object.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/result/bioinfo.py` & `geoseeq-0.5.6a9/geoseeq/result/bioinfo.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/result/file_download.py` & `geoseeq-0.5.6a9/geoseeq/result/file_download.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/result/file_upload.py` & `geoseeq-0.5.6a9/geoseeq/result/file_upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,18 +256,20 @@
             threads,
             resumable_upload_tracker=resumable_upload_tracker
         )
         self._finish_multipart_upload(upload_id, complete_parts)
         logger.info(f'Finished Upload for "{filepath}"')
         return self
 
-    def upload_file(self, filepath, multipart_thresh=FIVE_MB, overwrite=True, **kwargs):
+    def upload_file(self, filepath, multipart_thresh=FIVE_MB, overwrite=True, no_new_versions=False, **kwargs):
         if self.exists() and not overwrite:  
             raise GeoseeqGeneralError(f"Overwrite is set to False and file {self.uuid} already exists.")
         self.idem()
+        if no_new_versions and self.has_downloadable_file():
+            raise GeoseeqGeneralError(f"File {self} already has a downloadable file. Not uploading a new version.")
         resolved_path = Path(filepath).resolve()
         file_size = getsize(resolved_path)
         return self.multipart_upload_file(filepath, file_size, **kwargs)
     
     def upload_json(self, data, **kwargs):
         """Upload a file with the given data as JSON."""
         with NamedTemporaryFile("w", suffix='.json') as f:
```

### Comparing `geoseeq-0.5.6a8/geoseeq/result/result_file.py` & `geoseeq-0.5.6a9/geoseeq/result/result_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,22 @@
         return isinstance(self, SampleAnalysisResultField)
 
     @property
     def brn(self):
         obj_type = "sample" if self.canon_url() == "sample_ar_fields" else "project"
         brn = f"brn:{self.knex.instance_code()}:{obj_type}_result_field:{self.uuid}"
 
+    def has_downloadable_file(self):
+        """Return True if this field has a downloadable file."""
+        try:
+            self.download(head=10, cache=False)
+            return True
+        except Exception as e:
+            return False
+
     def nested_url(self):
         escaped_name = urllib.parse.quote(self.name, safe="")
         return self.parent.nested_url() + f"/fields/{escaped_name}"
 
     def get_blob_filename(self):
         sname = self.parent.parent.name.replace(".", "-")
         mname = self.parent.module_name.replace(".", "-")
```

### Comparing `geoseeq-0.5.6a8/geoseeq/result/result_folder.py` & `geoseeq-0.5.6a9/geoseeq/result/result_folder.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/result/utils.py` & `geoseeq-0.5.6a9/geoseeq/result/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/sample.py` & `geoseeq-0.5.6a9/geoseeq/sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/search.py` & `geoseeq-0.5.6a9/geoseeq/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/upload_download_manager.py` & `geoseeq-0.5.6a9/geoseeq/upload_download_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,42 +15,50 @@
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter('[%(levelname)s] %(name)s :: ' + current_process().name + ' :: %(message)s'))
     logger.addHandler(handler)
     return logger
 
 
 def _upload_one_file(args):
-    result_file, filepath, session, progress_tracker, link_type, overwrite, log_level, parallel_uploads, use_cache = args
+    (result_file, filepath, session, progress_tracker,
+     link_type, overwrite, log_level, parallel_uploads,
+     use_cache, no_new_versions) = args
     if parallel_uploads:
         _make_in_process_logger(log_level)
     if link_type == 'upload':
         # TODO: check checksums to see if the file is the same
-        result_file.upload_file(filepath, session=session, overwrite=overwrite, progress_tracker=progress_tracker, threads=4, use_cache=use_cache)
+        result_file.upload_file(
+            filepath,
+            session=session, overwrite=overwrite, progress_tracker=progress_tracker,
+            threads=4, use_cache=use_cache, no_new_versions=no_new_versions
+        )
     else:
         result_file.link_file(link_type, filepath)
     return result_file
 
 
 class GeoSeeqUploadManager:
 
     def __init__(self,
                  n_parallel_uploads=1,
                  session=None,
                  link_type='upload',
                  progress_tracker_factory=None,
                  log_level=logging.WARNING,
                  overwrite=True,
+                 no_new_versions=False,
                  use_cache=True):
         self.session = session
         self.n_parallel_uploads = n_parallel_uploads
         self.progress_tracker_factory = progress_tracker_factory if progress_tracker_factory else lambda x: None
         self.log_level = log_level
         self.link_type = link_type
         self.overwrite = overwrite
         self._result_files = []
+        self.no_new_versions = no_new_versions
         self.use_cache = use_cache
 
     def add_result_file(self, result_file, local_path):
         self._result_files.append((result_file, local_path))
 
     def add_local_file_to_result_folder(self, result_folder, local_path, geoseeq_file_name=None):
         geoseeq_file_name = geoseeq_file_name if geoseeq_file_name else local_path
@@ -68,15 +76,15 @@
         return "\n".join(out)
 
     def upload_files(self):
         upload_args = [(
                 result_file, local_path,
                 self.session, self.progress_tracker_factory(local_path),
                 self.link_type, self.overwrite, self.log_level,
-                self.n_parallel_uploads > 1, self.use_cache
+                self.n_parallel_uploads > 1, self.use_cache, self.no_new_versions
             ) for result_file, local_path in self._result_files
         ]
         out = []
         if self.n_parallel_uploads == 1:
             logger.info(f"Uploading files in series.")
             for upload_arg in upload_args:
                 out.append(_upload_one_file(upload_arg))
```

### Comparing `geoseeq-0.5.6a8/geoseeq/user.py` & `geoseeq-0.5.6a9/geoseeq/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/utils.py` & `geoseeq-0.5.6a9/geoseeq/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/vc/checksum.py` & `geoseeq-0.5.6a9/geoseeq/vc/checksum.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/vc/cli.py` & `geoseeq-0.5.6a9/geoseeq/vc/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/vc/clone.py` & `geoseeq-0.5.6a9/geoseeq/vc/clone.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/vc/vc_cache.py` & `geoseeq-0.5.6a9/geoseeq/vc/vc_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/vc/vc_sample.py` & `geoseeq-0.5.6a9/geoseeq/vc/vc_sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/vc/vc_stub.py` & `geoseeq-0.5.6a9/geoseeq/vc/vc_stub.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq/work_orders.py` & `geoseeq-0.5.6a9/geoseeq/work_orders.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/geoseeq.egg-info/PKG-INFO` & `geoseeq-0.5.6a9/geoseeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a8
+Version: 0.5.6a9
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a8/geoseeq.egg-info/SOURCES.txt` & `geoseeq-0.5.6a9/geoseeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/pyproject.toml` & `geoseeq-0.5.6a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geoseeq"
-version = "0.5.6a8"
+version = "0.5.6a9"
 authors = [
   { name="David C. Danko", email="dcdanko@biotia.io" },
 ]
 description = "GeoSeeq command line tools and python API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `geoseeq-0.5.6a8/setup.py` & `geoseeq-0.5.6a9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import setuptools
 
 setuptools.setup(
     name='geoseeq',
-    version='0.5.6a7',  # remember to update version string in CLI as well
+    version='0.5.6a7',  # DEPRECATED see pyproject.toml remember to update version string in CLI as well
     author="David C. Danko",
     author_email='dcdanko@biotia.io',
     description=open('README.md').read(),
     packages=setuptools.find_packages(),
     package_dir={'geoseeq': 'geoseeq'},
     install_requires=[
         'requests',
```

### Comparing `geoseeq-0.5.6a8/tests/test_api_client.py` & `geoseeq-0.5.6a9/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a8/tests/test_plotting.py` & `geoseeq-0.5.6a9/tests/test_plotting.py`

 * *Files identical despite different names*

