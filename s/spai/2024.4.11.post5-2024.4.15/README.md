# Comparing `tmp/spai-2024.4.11.post5.tar.gz` & `tmp/spai-2024.4.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2024.4.11.post5.tar", max compression
+gzip compressed data, was "spai-2024.4.15.tar", max compression
```

## Comparing `spai-2024.4.11.post5.tar` & `spai-2024.4.15.tar`

### file list

```diff
@@ -1,131 +1,132 @@
--rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2024.4.11.post5/README.md
--rw-r--r--   0        0        0      527 2024-04-11 14:55:52.414466 spai-2024.4.11.post5/pyproject.toml
--rw-r--r--   0        0        0       29 2024-04-11 14:55:52.414466 spai-2024.4.11.post5/spai/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/analytics/__init__.py
--rw-r--r--   0        0        0     5240 2024-04-11 14:55:43.286426 spai-2024.4.11.post5/spai/analytics/forest_monitoring.py
--rw-r--r--   0        0        0    12191 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/analytics/water_quality.py
--rw-r--r--   0        0        0       96 2024-02-13 11:22:06.401893 spai-2024.4.11.post5/spai/auth/__init__.py
--rw-r--r--   0        0        0     1210 2024-02-13 11:22:06.401893 spai-2024.4.11.post5/spai/auth/auth.py
--rw-r--r--   0        0        0       99 2024-02-13 11:22:06.401893 spai-2024.4.11.post5/spai/auth/is_logged.py
--rw-r--r--   0        0        0      161 2024-02-13 11:22:06.401893 spai-2024.4.11.post5/spai/auth/logout.py
--rw-r--r--   0        0        0     7202 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/cli.py
--rw-r--r--   0        0        0        0 2024-02-13 11:22:06.401893 spai-2024.4.11.post5/spai/commands/__init__.py
--rw-r--r--   0        0        0     1017 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/commands/auth.py
--rw-r--r--   0        0        0     1160 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/commands/list.py
--rw-r--r--   0        0        0       86 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/config/__init__.py
--rw-r--r--   0        0        0     3583 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/config/validate.py
--rw-r--r--   0        0        0     1324 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/config/vars.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2024.4.11.post5/spai/data/__init__.py
--rw-r--r--   0        0        0       49 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/indices/__init__.py
--rw-r--r--   0        0        0       54 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/indices/fwi/__init__.py
--rw-r--r--   0        0        0     3234 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/indices/fwi/fwi_nasa.py
--rw-r--r--   0        0        0      608 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     3941 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/satellite/download.py
--rw-r--r--   0        0        0     6332 2024-04-11 13:22:00.598259 spai-2024.4.11.post5/spai/data/satellite/download_stac.py
--rw-r--r--   0        0        0      647 2023-10-30 11:07:40.852696 spai-2024.4.11.post5/spai/data/satellite/explore.py
--rw-r--r--   0        0        0      725 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
--rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
--rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
--rw-r--r--   0        0        0      758 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
--rw-r--r--   0        0        0     3587 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2584 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1264 2023-10-30 11:07:40.856696 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      282 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0     2222 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/STACDownloader.py
--rw-r--r--   0        0        0      208 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/__init__.py
--rw-r--r--   0        0        0      461 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/aws/AWSDEM30Downloader.py
--rw-r--r--   0        0        0      461 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/aws/AWSDEM90Downloader.py
--rw-r--r--   0        0        0      876 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/aws/AWSDEMDownloader.py
--rw-r--r--   0        0        0      392 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/aws/AWSDownloader.py
--rw-r--r--   0        0        0     1951 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py
--rw-r--r--   0        0        0      233 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/aws/__init__.py
--rw-r--r--   0        0        0      456 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/decorators.py
--rw-r--r--   0        0        0      716 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/pc/PCDownloader.py
--rw-r--r--   0        0        0      802 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/pc/PCS1GRDDownloader.py
--rw-r--r--   0        0        0      120 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/stac/pc/__init__.py
--rw-r--r--   0        0        0     8905 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/data/satellite/utils.py
--rw-r--r--   0        0        0       84 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/vector/__init__.py
--rw-r--r--   0        0        0     5533 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/data/vector/openstreetmap.py
--rw-r--r--   0        0        0       71 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/errors/__init__.py
--rw-r--r--   0        0        0      308 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/errors/auth.py
--rw-r--r--   0        0        0      156 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/errors/mails.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2024.4.11.post5/spai/image/__init__.py
--rw-r--r--   0        0        0     1350 2023-10-30 11:07:40.856696 spai-2024.4.11.post5/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2024.4.11.post5/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2024.4.11.post5/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2024.4.11.post5/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2024.4.11.post5/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2024.4.11.post5/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0       28 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/mails/__init__.py
--rw-r--r--   0        0        0     1334 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/mails/mimetypes.py
--rw-r--r--   0        0        0     2932 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/mails/send.py
--rw-r--r--   0        0        0     3305 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/models/Config.py
--rw-r--r--   0        0        0      984 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/models/StorageConfig.py
--rw-r--r--   0        0        0       27 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/models/__init__.py
--rw-r--r--   0        0        0      391 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/processing/__init__.py
--rw-r--r--   0        0        0      669 2024-03-28 15:02:41.834449 spai-2024.4.11.post5/spai/processing/autocategorize1D.py
--rw-r--r--   0        0        0      477 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/processing/colorize_raster.py
--rw-r--r--   0        0        0      932 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/processing/convert_array_to_vector.py
--rw-r--r--   0        0        0      291 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/processing/mask_raster.py
--rw-r--r--   0        0        0      682 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/processing/normalised_difference.py
--rw-r--r--   0        0        0     1239 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/processing/px_count.py
--rw-r--r--   0        0        0      107 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/processing/rasterio_mask.py
--rw-r--r--   0        0        0      266 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/processing/read_raster.py
--rw-r--r--   0        0        0      876 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/processing/save_table.py
--rw-r--r--   0        0        0      496 2024-03-28 15:02:41.834449 spai-2024.4.11.post5/spai/processing/utils.py
--rw-r--r--   0        0        0      475 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/__init__.py
--rw-r--r--   0        0        0      466 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/bck/GetLogs.py
--rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/project/bck/InstallReqs 2.py
--rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/project/bck/InstallReqs 3.py
--rw-r--r--   0        0        0      482 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/bck/RunService.py
--rw-r--r--   0        0        0      492 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/bck/ScheduleService.py
--rw-r--r--   0        0        0      510 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/bck/StopService.py
--rw-r--r--   0        0        0     1578 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/bck/main.py
--rw-r--r--   0        0        0      337 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/delete_project.py
--rw-r--r--   0        0        0     2060 2024-03-28 15:01:17.074615 spai-2024.4.11.post5/spai/project/deploy_folder.py
--rw-r--r--   0        0        0      408 2024-03-28 15:01:17.078615 spai-2024.4.11.post5/spai/project/deploy_template.py
--rw-r--r--   0        0        0     1203 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/download_template.py
--rw-r--r--   0        0        0      455 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/get_logs.py
--rw-r--r--   0        0        0      242 2024-02-13 11:22:06.405893 spai-2024.4.11.post5/spai/project/get_project_by_name.py
--rw-r--r--   0        0        0      172 2024-02-13 11:22:06.409893 spai-2024.4.11.post5/spai/project/get_projects.py
--rw-r--r--   0        0        0      344 2024-02-13 11:22:06.409893 spai-2024.4.11.post5/spai/project/get_service_by_name_type_project.py
--rw-r--r--   0        0        0     1616 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/project/get_services.py
--rw-r--r--   0        0        0      525 2024-02-21 09:43:40.417670 spai-2024.4.11.post5/spai/project/init_project.py
--rw-r--r--   0        0        0      726 2024-02-20 15:56:19.617848 spai-2024.4.11.post5/spai/project/install_requirements.py
--rw-r--r--   0        0        0     5617 2024-02-27 12:31:33.913016 spai-2024.4.11.post5/spai/project/project-template/README.md
--rw-r--r--   0        0        0      867 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/project/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0       36 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/project/project-template/apis/analytics/requirements.txt
--rw-r--r--   0        0        0     1800 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/project/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0       88 2024-03-13 09:12:15.507871 spai-2024.4.11.post5/spai/project/project-template/apis/xyz/requirements.txt
--rw-r--r--   0        0        0   748531 2024-03-13 09:12:15.511871 spai-2024.4.11.post5/spai/project/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0       39 2024-03-13 09:12:15.511871 spai-2024.4.11.post5/spai/project/project-template/notebooks/analytics/requirements.txt
--rw-r--r--   0        0        0     1602 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/project/project-template/scripts/analytics/main.py
--rw-r--r--   0        0        0       30 2024-03-13 09:12:15.511871 spai-2024.4.11.post5/spai/project/project-template/scripts/analytics/requirements.txt
--rw-r--r--   0        0        0     1076 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/project/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0       85 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/project/project-template/scripts/downloader/requirements.txt
--rw-r--r--   0        0        0      618 2024-03-13 09:12:15.511871 spai-2024.4.11.post5/spai/project/project-template/spai.config.yaml
--rw-r--r--   0        0        0     1523 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/project/project-template/uis/map/main.py
--rw-r--r--   0        0        0       23 2024-02-27 12:31:33.593015 spai-2024.4.11.post5/spai/project/project-template/uis/map/requirements.txt
--rw-r--r--   0        0        0     5242 2024-03-25 08:56:48.420217 spai-2024.4.11.post5/spai/project/run_local.py
--rw-r--r--   0        0        0      813 2024-03-13 09:12:15.511871 spai-2024.4.11.post5/spai/project/stop_service.py
--rw-r--r--   0        0        0       38 2024-02-13 11:22:06.413893 spai-2024.4.11.post5/spai/reports/__init__.py
--rw-r--r--   0        0        0     1328 2024-02-13 11:22:06.413893 spai-2024.4.11.post5/spai/reports/generate.py
--rw-r--r--   0        0        0     4709 2024-03-13 09:12:15.511871 spai-2024.4.11.post5/spai/repos/APIRepo.py
--rw-r--r--   0        0        0      997 2024-02-13 11:22:06.413893 spai-2024.4.11.post5/spai/repos/AuthRepo.py
--rw-r--r--   0        0        0      188 2024-02-13 11:22:06.413893 spai-2024.4.11.post5/spai/repos/MailsRepo.py
--rw-r--r--   0        0        0      200 2024-02-13 11:22:06.413893 spai-2024.4.11.post5/spai/repos/ReportsRepo.py
--rw-r--r--   0        0        0       60 2024-02-13 11:22:06.413893 spai-2024.4.11.post5/spai/repos/__init__.py
--rw-r--r--   0        0        0     2452 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3716 2024-03-13 09:12:15.515871 spai-2024.4.11.post5/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     4527 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/storage/LocalStorage.py
--rw-r--r--   0        0        0     8449 2024-04-11 11:16:27.098890 spai-2024.4.11.post5/spai/storage/S3Storage.py
--rw-r--r--   0        0        0     1407 2024-03-13 09:12:15.515871 spai-2024.4.11.post5/spai/storage/Storage.py
--rw-r--r--   0        0        0     6077 2024-03-13 09:12:15.515871 spai-2024.4.11.post5/spai/storage/_S3Storage.py
--rw-r--r--   0        0        0      120 2024-03-13 09:12:15.515871 spai-2024.4.11.post5/spai/storage/__init__.py
--rw-r--r--   0        0        0      409 2024-03-13 09:12:15.515871 spai-2024.4.11.post5/spai/storage/create_s3.py
--rw-r--r--   0        0        0     1559 2024-04-11 11:16:27.102890 spai-2024.4.11.post5/spai/storage/decorators.py
--rw-r--r--   0        0        0      583 2024-03-13 09:12:15.515871 spai-2024.4.11.post5/spai/storage/minio.py
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 spai-2024.4.11.post5/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2024.4.15/README.md
+-rw-r--r--   0        0        0      525 2024-04-15 09:35:58.009182 spai-2024.4.15/pyproject.toml
+-rw-r--r--   0        0        0       27 2024-04-15 09:35:58.009182 spai-2024.4.15/spai/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/analytics/__init__.py
+-rw-r--r--   0        0        0     5030 2024-04-12 10:11:53.821360 spai-2024.4.15/spai/analytics/forest_monitoring.py
+-rw-r--r--   0        0        0      110 2024-04-12 10:11:53.821360 spai-2024.4.15/spai/analytics/utils.py
+-rw-r--r--   0        0        0    13235 2024-04-12 10:11:53.821360 spai-2024.4.15/spai/analytics/water_quality.py
+-rw-r--r--   0        0        0       96 2024-02-13 11:22:06.401893 spai-2024.4.15/spai/auth/__init__.py
+-rw-r--r--   0        0        0     1210 2024-02-13 11:22:06.401893 spai-2024.4.15/spai/auth/auth.py
+-rw-r--r--   0        0        0       99 2024-02-13 11:22:06.401893 spai-2024.4.15/spai/auth/is_logged.py
+-rw-r--r--   0        0        0      161 2024-02-13 11:22:06.401893 spai-2024.4.15/spai/auth/logout.py
+-rw-r--r--   0        0        0     7202 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/cli.py
+-rw-r--r--   0        0        0        0 2024-02-13 11:22:06.401893 spai-2024.4.15/spai/commands/__init__.py
+-rw-r--r--   0        0        0     1017 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/commands/auth.py
+-rw-r--r--   0        0        0     1160 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/commands/list.py
+-rw-r--r--   0        0        0       86 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/config/__init__.py
+-rw-r--r--   0        0        0     3583 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/config/validate.py
+-rw-r--r--   0        0        0     1324 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/config/vars.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2024.4.15/spai/data/__init__.py
+-rw-r--r--   0        0        0       49 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/indices/__init__.py
+-rw-r--r--   0        0        0       54 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/indices/fwi/__init__.py
+-rw-r--r--   0        0        0     3234 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/indices/fwi/fwi_nasa.py
+-rw-r--r--   0        0        0      608 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     3941 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     6332 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/download_stac.py
+-rw-r--r--   0        0        0      647 2023-10-30 11:07:40.852696 spai-2024.4.15/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0      725 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py
+-rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py
+-rw-r--r--   0        0        0      758 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py
+-rw-r--r--   0        0        0      758 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/satellite/sentinelhub/SHDEM30Downloader.py
+-rw-r--r--   0        0        0     3587 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2584 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2024.4.15/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1264 2023-10-30 11:07:40.856696 spai-2024.4.15/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2024.4.15/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2024.4.15/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      282 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     2222 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/STACDownloader.py
+-rw-r--r--   0        0        0      208 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/__init__.py
+-rw-r--r--   0        0        0      461 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/aws/AWSDEM30Downloader.py
+-rw-r--r--   0        0        0      461 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/aws/AWSDEM90Downloader.py
+-rw-r--r--   0        0        0      876 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/aws/AWSDEMDownloader.py
+-rw-r--r--   0        0        0      392 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/aws/AWSDownloader.py
+-rw-r--r--   0        0        0     1951 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py
+-rw-r--r--   0        0        0      233 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/aws/__init__.py
+-rw-r--r--   0        0        0      456 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/decorators.py
+-rw-r--r--   0        0        0      716 2024-04-12 10:11:48.513337 spai-2024.4.15/spai/data/satellite/stac/pc/PCDownloader.py
+-rw-r--r--   0        0        0      802 2024-04-12 10:11:48.517337 spai-2024.4.15/spai/data/satellite/stac/pc/PCS1GRDDownloader.py
+-rw-r--r--   0        0        0      120 2024-04-11 11:16:27.098890 spai-2024.4.15/spai/data/satellite/stac/pc/__init__.py
+-rw-r--r--   0        0        0     8905 2024-04-12 10:11:48.517337 spai-2024.4.15/spai/data/satellite/utils.py
+-rw-r--r--   0        0        0       84 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/vector/__init__.py
+-rw-r--r--   0        0        0     5533 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/data/vector/openstreetmap.py
+-rw-r--r--   0        0        0       71 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/errors/__init__.py
+-rw-r--r--   0        0        0      308 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/errors/auth.py
+-rw-r--r--   0        0        0      156 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/errors/mails.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2024.4.15/spai/image/__init__.py
+-rw-r--r--   0        0        0     1350 2023-10-30 11:07:40.856696 spai-2024.4.15/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2024.4.15/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2024.4.15/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2024.4.15/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2024.4.15/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2024.4.15/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0       28 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/mails/__init__.py
+-rw-r--r--   0        0        0     1334 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/mails/mimetypes.py
+-rw-r--r--   0        0        0     2932 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/mails/send.py
+-rw-r--r--   0        0        0     3305 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/models/Config.py
+-rw-r--r--   0        0        0      984 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/models/StorageConfig.py
+-rw-r--r--   0        0        0       27 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/models/__init__.py
+-rw-r--r--   0        0        0      391 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/processing/__init__.py
+-rw-r--r--   0        0        0      669 2024-03-28 15:02:41.834449 spai-2024.4.15/spai/processing/autocategorize1D.py
+-rw-r--r--   0        0        0      477 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/processing/colorize_raster.py
+-rw-r--r--   0        0        0      932 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/processing/convert_array_to_vector.py
+-rw-r--r--   0        0        0      291 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/processing/mask_raster.py
+-rw-r--r--   0        0        0      682 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/processing/normalised_difference.py
+-rw-r--r--   0        0        0     1239 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/processing/px_count.py
+-rw-r--r--   0        0        0      107 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/processing/rasterio_mask.py
+-rw-r--r--   0        0        0      266 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/processing/read_raster.py
+-rw-r--r--   0        0        0     1109 2024-04-12 10:11:53.821360 spai-2024.4.15/spai/processing/save_table.py
+-rw-r--r--   0        0        0      496 2024-03-28 15:02:41.834449 spai-2024.4.15/spai/processing/utils.py
+-rw-r--r--   0        0        0      475 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/__init__.py
+-rw-r--r--   0        0        0      466 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/bck/GetLogs.py
+-rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/project/bck/InstallReqs 2.py
+-rw-r--r--   0        0        0     1018 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/project/bck/InstallReqs 3.py
+-rw-r--r--   0        0        0      482 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/bck/RunService.py
+-rw-r--r--   0        0        0      492 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/bck/ScheduleService.py
+-rw-r--r--   0        0        0      510 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/bck/StopService.py
+-rw-r--r--   0        0        0     1578 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/bck/main.py
+-rw-r--r--   0        0        0      337 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/delete_project.py
+-rw-r--r--   0        0        0     2064 2024-04-15 08:23:54.593387 spai-2024.4.15/spai/project/deploy_folder.py
+-rw-r--r--   0        0        0      410 2024-04-15 08:23:54.593387 spai-2024.4.15/spai/project/deploy_template.py
+-rw-r--r--   0        0        0     1203 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/download_template.py
+-rw-r--r--   0        0        0      455 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/get_logs.py
+-rw-r--r--   0        0        0      242 2024-02-13 11:22:06.405893 spai-2024.4.15/spai/project/get_project_by_name.py
+-rw-r--r--   0        0        0      172 2024-02-13 11:22:06.409893 spai-2024.4.15/spai/project/get_projects.py
+-rw-r--r--   0        0        0      344 2024-02-13 11:22:06.409893 spai-2024.4.15/spai/project/get_service_by_name_type_project.py
+-rw-r--r--   0        0        0     1616 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/project/get_services.py
+-rw-r--r--   0        0        0      525 2024-02-21 09:43:40.417670 spai-2024.4.15/spai/project/init_project.py
+-rw-r--r--   0        0        0      726 2024-02-20 15:56:19.617848 spai-2024.4.15/spai/project/install_requirements.py
+-rw-r--r--   0        0        0     5617 2024-02-27 12:31:33.913016 spai-2024.4.15/spai/project/project-template/README.md
+-rw-r--r--   0        0        0      867 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/project/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0       36 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/project/project-template/apis/analytics/requirements.txt
+-rw-r--r--   0        0        0     1800 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/project/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0       88 2024-03-13 09:12:15.507871 spai-2024.4.15/spai/project/project-template/apis/xyz/requirements.txt
+-rw-r--r--   0        0        0   748531 2024-03-13 09:12:15.511871 spai-2024.4.15/spai/project/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0       39 2024-03-13 09:12:15.511871 spai-2024.4.15/spai/project/project-template/notebooks/analytics/requirements.txt
+-rw-r--r--   0        0        0     1602 2024-04-12 10:11:48.517337 spai-2024.4.15/spai/project/project-template/scripts/analytics/main.py
+-rw-r--r--   0        0        0       30 2024-03-13 09:12:15.511871 spai-2024.4.15/spai/project/project-template/scripts/analytics/requirements.txt
+-rw-r--r--   0        0        0     1076 2024-04-12 10:11:48.517337 spai-2024.4.15/spai/project/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0       85 2024-04-12 10:11:48.517337 spai-2024.4.15/spai/project/project-template/scripts/downloader/requirements.txt
+-rw-r--r--   0        0        0      618 2024-03-13 09:12:15.511871 spai-2024.4.15/spai/project/project-template/spai.config.yaml
+-rw-r--r--   0        0        0     1523 2024-04-12 10:11:48.517337 spai-2024.4.15/spai/project/project-template/uis/map/main.py
+-rw-r--r--   0        0        0       23 2024-02-27 12:31:33.593015 spai-2024.4.15/spai/project/project-template/uis/map/requirements.txt
+-rw-r--r--   0        0        0     5242 2024-03-25 08:56:48.420217 spai-2024.4.15/spai/project/run_local.py
+-rw-r--r--   0        0        0      813 2024-03-13 09:12:15.511871 spai-2024.4.15/spai/project/stop_service.py
+-rw-r--r--   0        0        0       38 2024-02-13 11:22:06.413893 spai-2024.4.15/spai/reports/__init__.py
+-rw-r--r--   0        0        0     1328 2024-02-13 11:22:06.413893 spai-2024.4.15/spai/reports/generate.py
+-rw-r--r--   0        0        0     4709 2024-03-13 09:12:15.511871 spai-2024.4.15/spai/repos/APIRepo.py
+-rw-r--r--   0        0        0      997 2024-02-13 11:22:06.413893 spai-2024.4.15/spai/repos/AuthRepo.py
+-rw-r--r--   0        0        0      188 2024-02-13 11:22:06.413893 spai-2024.4.15/spai/repos/MailsRepo.py
+-rw-r--r--   0        0        0      200 2024-02-13 11:22:06.413893 spai-2024.4.15/spai/repos/ReportsRepo.py
+-rw-r--r--   0        0        0       60 2024-02-13 11:22:06.413893 spai-2024.4.15/spai/repos/__init__.py
+-rw-r--r--   0        0        0     2448 2024-04-15 09:35:35.141035 spai-2024.4.15/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3716 2024-03-13 09:12:15.515871 spai-2024.4.15/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     4527 2024-04-11 11:16:27.098890 spai-2024.4.15/spai/storage/LocalStorage.py
+-rw-r--r--   0        0        0     8449 2024-04-12 10:11:48.517337 spai-2024.4.15/spai/storage/S3Storage.py
+-rw-r--r--   0        0        0     1407 2024-03-13 09:12:15.515871 spai-2024.4.15/spai/storage/Storage.py
+-rw-r--r--   0        0        0     6077 2024-03-13 09:12:15.515871 spai-2024.4.15/spai/storage/_S3Storage.py
+-rw-r--r--   0        0        0      120 2024-03-13 09:12:15.515871 spai-2024.4.15/spai/storage/__init__.py
+-rw-r--r--   0        0        0      409 2024-03-13 09:12:15.515871 spai-2024.4.15/spai/storage/create_s3.py
+-rw-r--r--   0        0        0     1559 2024-04-11 11:16:27.102890 spai-2024.4.15/spai/storage/decorators.py
+-rw-r--r--   0        0        0      583 2024-03-13 09:12:15.515871 spai-2024.4.15/spai/storage/minio.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 spai-2024.4.15/PKG-INFO
```

### Comparing `spai-2024.4.11.post5/pyproject.toml` & `spai-2024.4.15/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spai"
-version = "2024.04.11-5"
+version = "2024.04.15"
 description = ""
 authors = ["Juan Sensio <it@earthpulse.es>"]
 readme = "README.md"
 packages = [{include = "spai"}]
 
 [tool.poetry.scripts]
 spai = "spai.cli:app"
```

### Comparing `spai-2024.4.11.post5/spai/analytics/forest_monitoring.py` & `spai-2024.4.15/spai/analytics/forest_monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 from ..processing import normalised_difference
 from ..processing import mask_raster
 from ..processing import autocategorize1D
 from ..processing import px_count
 from ..processing import colorize_raster
 from ..processing import save_table
 
-
-def format_name(name, prefix, date):
-    return prefix + name.format(date=date)
+from .utils import format_name
 
 
 def forest_monitoring(
     image_name,
+    date,
     aoi_mask,
     storage,
     prefix="",  # prefix for the raster names
     names={},
 ):
     default_names = {  # names for the raster files
         "ndvi": "ndvi_{date}.tif",
@@ -34,18 +33,14 @@
         "vegetation_quality": "AOI_Vegetation_Quality.json",
     }
     names = {**default_names, **names}
 
     # read_raster image
     ds, raster = read_raster(image_name, storage)
 
-    # esto no siempre va a funcionar... si el nombre de la imagen no sigue el formato
-    date_and_tif = image_name.split("_")[-1]
-    date = date_and_tif.split(".")[0]
-
     # calculate ndvi
     ndvi = normalised_difference(raster)
 
     # save_raster ndvi
     raster_name_ndvi = format_name(names["ndvi"], prefix, date)
     storage.create(ndvi, raster_name_ndvi, ds=ds)
```

### Comparing `spai-2024.4.11.post5/spai/analytics/water_quality.py` & `spai-2024.4.15/spai/analytics/water_quality.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from ..processing import read_raster
 from ..processing import colorize_raster
 from ..processing import px_count
 from ..processing import save_table
 from ..processing import normalised_difference
 from ..processing import convert_array_to_vector
 
+from .utils import format_name
 
-def water_quality(image_name, aoi_mask, storage, date=None):
+
+def water_quality(image_name, date, storage, prefix="", names={}):
     """
     This function calculates the water quality of a given image.
 
     It calculates the following layers:
         - Normalized Difference Water Index (NDWI) - ndwi_{date}.tif, ndwi_masked_{date}.tif, ndwi_categorized_{date}.tif
         - Normalized Difference Turbidity Index (NDTI) - ndti_{date}.tif, ndti_masked_{date}.tif, ndti_categorized_{date}.tif
         - Normalized Difference Chlorophyll Index (NDCI) - ndci_{date}.tif, ndci_masked_{date}.tif, ndci_categorized_{date}.tif
@@ -31,119 +33,138 @@
         - Water Chlorophyll (in hectares and percentage) - table_chlorophyll_Ha.json, table_chlorophyll_percent.json
         - Water DOC (in hectares and percentage) - table_DOC_Ha.json, table_DOC_percent.json
 
     Parameters
     ----------
     image_name : str
         The name of the image to be processed.
-    aoi_mask : dict
-        The GeoJSON of the area of interest.
+    date: str
+        The date of the image to be processed.
     storage : Storage
         The Storage object.
-    date : str, optional
-        The date of the image from which start downloading earlier images to determine the water body status,
-        by default None, which uses the date given in the image name.
 
     Returns
     -------
     None
 
     """
+    default_names = {
+        "ndwi": "ndwi_{date}.tif",
+        "ndwi_masked": "ndwi_masked_{date}.tif",
+        "ndwi_categorized": "ndwi_categorized_{date}.tif",
+        "ndti": "ndti_{date}.tif",
+        "ndti_masked": "ndti_masked_{date}.tif",
+        "ndti_categorized": "ndti_categorized_{date}.tif",
+        "ndti_categorized_rgb": "ndti_categorized_rgb_{date}.tif",
+        "ndci": "ndci_{date}.tif",
+        "ndci_masked": "ndci_masked_{date}.tif",
+        "ndci_categorized": "ndci_categorized_{date}.tif",
+        "ndci_categorized_rgb": "ndci_categorized_rgb_{date}.tif",
+        "water_mask": "water_mask_{date}.tif",
+        "DOC": "DOC_{date}.tif",
+        "DOC_masked": "DOC_masked_{date}.tif",
+        "DOC_categorized": "DOC_categorized_{date}.tif",
+        "DOC_categorized_rgb": "DOC_categorized_rgb_{date}.tif",
+    }
+    names = {**default_names, **names}
+
     # read_raster image
     ds, raster = read_raster(image_name, storage, bands=[3, 4, 5, 8])
-    date = image_name.split(".")[0].split("_")[-1]
 
     """ LAYERS """
     # NDWI
 
     # calculate ndwi
     ndwi = normalised_difference(raster, [1, 4])
 
     # save_raster ndwi
-    raster_name_ndwi = f"ndwi_{date}.tif"
+    raster_name_ndwi = format_name(names["ndwi"], prefix, date)
+    print(raster_name_ndwi)
     storage.create(ndwi, raster_name_ndwi, ds=ds)
 
     # NDTI
     # calculate ndti
     ndti = normalised_difference(raster, [2, 1])
 
     # save_raster ndti
-    raster_name_ndti = f"ndti_{date}.tif"
+    raster_name_ndti = format_name(names["ndti"], prefix, date)
     storage.create(ndti, raster_name_ndti, ds=ds)
 
     # NDCI
     # calculate ndci
     ndci = normalised_difference(raster, [3, 2])
     ndci = equalize_hist(ndci)
 
     # save_raster ndci
-    raster_name_ndci = f"ndci_{date}.tif"
+    raster_name_ndci = format_name(names["ndci"], prefix, date)
     storage.create(ndci, raster_name_ndci, ds=ds)
 
     # Calculate water mask and smooth it
     # threshold on 0
     water_mask = ndwi >= 0.2
     water_mask = median_filter(water_mask, size=(10, 5))
 
     # save_raster water_mask
-    raster_name_water_mask = f"water_mask_{date}.tif"
+    raster_name_water_mask = format_name(names["water_mask"], prefix, date)
     storage.create(water_mask, raster_name_water_mask, ds=ds)
 
     # DOC
     # calculate doc
     stored_images = storage.list("sentinel-2-l2a*.tif")
     doc_layers_array, doc_values_array, ds = compute_doc(stored_images, storage)
 
     # save_raster doc
-    raster_name_doc = f"DOC_{date}.tif"
+    raster_name_doc = format_name(names["DOC"], prefix, date)
     storage.create(doc_layers_array[0], raster_name_doc, ds=ds)
 
     """ MASK LAYERS """
     shp = convert_array_to_vector(water_mask, storage.get_path(raster_name_water_mask))
 
     # mask_raster ndwi with aoi_mask
     ndwi_masked, _ = mask_raster(raster_name_ndwi, shp, storage)
 
     # save_raster ndwi_masked
-    raster_name_ndwi_masked = f"ndwi_masked_{date}.tif"
+    raster_name_ndwi_masked = format_name(names["ndwi_masked"], prefix, date)
     storage.create(ndwi_masked, raster_name_ndwi_masked, ds=ds)
 
     # mask_raster ndti with aoi_mask
     ndti_masked, _ = mask_raster(raster_name_ndti, shp, storage)
 
     # save_raster ndti_masked
-    raster_name_ndti_masked = f"ndti_masked_{date}.tif"
+    raster_name_ndti_masked = format_name(names["ndti_masked"], prefix, date)
     storage.create(ndti_masked, raster_name_ndti_masked, ds=ds)
 
     # mask_raster ndci with aoi_mask
     ndci_masked, _ = mask_raster(raster_name_ndci, shp, storage)
 
     # save_raster ndci_masked
-    raster_name_ndci_masked = f"ndci_masked_{date}.tif"
+    raster_name_ndci_masked = format_name(names["ndci_masked"], prefix, date)
     storage.create(ndci_masked, raster_name_ndci_masked, ds=ds)
 
     # mask_raster doc with aoi_mask
     doc_masked, _ = mask_raster(raster_name_doc, shp, storage)
 
     # save_raster doc_masked
-    raster_name_doc_masked = f"DOC_masked_{date}.tif"
+    raster_name_doc_masked = format_name(names["DOC_masked"], prefix, date)
     storage.create(doc_masked, raster_name_doc_masked, ds=ds)
 
     """ ANALYTICS """
     # Water Extent
     extent_has = np.divide(water_mask.sum().max(), 100)
     update_extent_table(extent_has, date, storage)
 
     # Water Turbidity
     ndti_categories = np.digitize(ndti_masked, [-np.inf, -0.2, 0.4, np.inf])
-    raster_name_ndti_categorized = f"ndti_categorized_{date}.tif"
+    raster_name_ndti_categorized = format_name(names["ndti_categorized"], prefix, date)
     storage.create(ndti_categories, raster_name_ndti_categorized, ds=ds)
 
     ndti_colorized = colorize_raster(ndti_categories, colors=["green", "yellow", "red"])
-    raster_name_ndti_colorized = f"ndti_categorized_rgb_{date}.tif"
+    raster_name_ndti_colorized = format_name(
+        names["ndti_categorized_rgb"], prefix, date
+    )
     storage.create(ndti_colorized, raster_name_ndti_colorized, ds=ds)
 
     ndti_px_counted = px_count(ndti_categories, [1, 2, 3])
     ndti_has = np.divide(
         ndti_px_counted,
         100,
         out=np.zeros_like(ndti_px_counted, dtype=np.float64),
@@ -171,19 +192,21 @@
         table_name=turbidity_percent_table_name,
         date=date,
         storage=storage,
     )
 
     # Water Chlorophyll
     ndci_categories = np.digitize(ndci_masked, [-np.inf, -0.3, 0.5, np.inf])
-    raster_name_ndci_categorized = f"ndci_categorized_{date}.tif"
+    raster_name_ndci_categorized = format_name(names["ndci_categorized"], prefix, date)
     storage.create(ndci_categories, raster_name_ndci_categorized, ds=ds)
 
     ndci_colorized = colorize_raster(ndci_categories, colors=["green", "yellow", "red"])
-    raster_name_ndci_colorized = f"ndci_categorized_rgb_{date}.tif"
+    raster_name_ndci_colorized = format_name(
+        names["ndci_categorized_rgb"], prefix, date
+    )
     storage.create(ndci_colorized, raster_name_ndci_colorized, ds=ds)
 
     ndci_px_counted = px_count(ndci_categories, [1, 2, 3])
     ndci_has = np.divide(
         ndci_px_counted,
         100,
         out=np.zeros_like(ndci_px_counted, dtype=np.float64),
@@ -224,19 +247,19 @@
     a = 1
     min_to_N0 = -np.inf
     N0_to_N1 = mean_mean_doc + 2 * mean_std_doc / a
     N1_to_N3 = mean_mean_doc + 4 * mean_std_doc / a
     N3_to_max = np.inf
 
     doc_categories = np.digitize(doc_masked, [min_to_N0, N0_to_N1, N1_to_N3, N3_to_max])
-    raster_name_doc_categorized = f"DOC_categorized_{date}.tif"
+    raster_name_doc_categorized = format_name(names["DOC_categorized"], prefix, date)
     storage.create(doc_categories, raster_name_doc_categorized, ds=ds)
 
     doc_colorized = colorize_raster(doc_categories, colors=["green", "yellow", "red"])
-    raster_name_doc_colorized = f"DOC_categorized_rgb_{date}.tif"
+    raster_name_doc_colorized = format_name(names["DOC_categorized_rgb"], prefix, date)
     storage.create(doc_colorized, raster_name_doc_colorized, ds=ds)
 
     doc_px_counted = px_count(doc_categories, [1, 2, 3])
     doc_has = np.divide(
         doc_px_counted,
         100,
         out=np.zeros_like(doc_px_counted, dtype=np.float64),
```

### Comparing `spai-2024.4.11.post5/spai/auth/auth.py` & `spai-2024.4.15/spai/auth/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/cli.py` & `spai-2024.4.15/spai/cli.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/commands/auth.py` & `spai-2024.4.15/spai/commands/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/commands/list.py` & `spai-2024.4.15/spai/commands/list.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/config/validate.py` & `spai-2024.4.15/spai/config/validate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/config/vars.py` & `spai-2024.4.15/spai/config/vars.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/indices/fwi/fwi_nasa.py` & `spai-2024.4.15/spai/data/indices/fwi/fwi_nasa.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/__init__.py` & `spai-2024.4.15/spai/data/satellite/__init__.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/download.py` & `spai-2024.4.15/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/download_stac.py` & `spai-2024.4.15/spai/data/satellite/download_stac.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/explore.py` & `spai-2024.4.15/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py` & `spai-2024.4.15/spai/data/satellite/sentinelhub/SHCloudMaskDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py` & `spai-2024.4.15/spai/data/satellite/sentinelhub/SHDEM30Downloader 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py` & `spai-2024.4.15/spai/data/satellite/sentinelhub/SHDEM30Downloader 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHDEM30Downloader.py` & `spai-2024.4.15/spai/data/satellite/sentinelhub/SHDEM30Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2024.4.15/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2024.4.15/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2024.4.15/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2024.4.15/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/stac/STACDownloader.py` & `spai-2024.4.15/spai/data/satellite/stac/STACDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/stac/aws/AWSDEMDownloader.py` & `spai-2024.4.15/spai/data/satellite/stac/aws/AWSDEMDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py` & `spai-2024.4.15/spai/data/satellite/stac/aws/AWSS2L2ADownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/stac/pc/PCDownloader.py` & `spai-2024.4.15/spai/data/satellite/stac/pc/PCDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/stac/pc/PCS1GRDDownloader.py` & `spai-2024.4.15/spai/data/satellite/stac/pc/PCS1GRDDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/satellite/utils.py` & `spai-2024.4.15/spai/data/satellite/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/data/vector/openstreetmap.py` & `spai-2024.4.15/spai/data/vector/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/image/utils.py` & `spai-2024.4.15/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/image/xyz/cache.py` & `spai-2024.4.15/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/image/xyz/errors.py` & `spai-2024.4.15/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/image/xyz/get_image_tile.py` & `spai-2024.4.15/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/image/xyz/image_utils.py` & `spai-2024.4.15/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/mails/mimetypes.py` & `spai-2024.4.15/spai/mails/mimetypes.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/mails/send.py` & `spai-2024.4.15/spai/mails/send.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/models/Config.py` & `spai-2024.4.15/spai/models/Config.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/models/StorageConfig.py` & `spai-2024.4.15/spai/models/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/processing/autocategorize1D.py` & `spai-2024.4.15/spai/processing/autocategorize1D.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/processing/convert_array_to_vector.py` & `spai-2024.4.15/spai/processing/convert_array_to_vector.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/processing/normalised_difference.py` & `spai-2024.4.15/spai/processing/normalised_difference.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/processing/px_count.py` & `spai-2024.4.15/spai/processing/px_count.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/processing/save_table.py` & `spai-2024.4.15/spai/processing/save_table.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,31 @@
 
 
 def save_table(data, columns, table_name, date, storage):
     # columns number must be equal to data number of columns
     if len(columns) != len(data):
         raise ValueError("columns number must be equal to data number of columns")
     # check if table exists in storage
+    # if table exists, append data to table
+    # if table does not exist, create table with data
     if table_name in storage.list():
-        # append data to table
         base_df = storage.read(table_name)
+
+        # Handle pd.DateTimeIndex, converting index to string
         if isinstance(base_df.index, pd.DatetimeIndex):
-            # Handle pd.DateTimeIndex, converting index to string
             base_df.index = base_df.index.strftime("%Y-%m-%d")
+
+        # Check if date already exists in table
+        if date in base_df.index:
+            base_df.drop(index=date, inplace=True)
+
         df = pd.concat(
             [pd.DataFrame([data], columns=columns, index=[date]), base_df.loc[:]]
         )
     else:
         # create table with data
         df = pd.DataFrame([data], columns=columns, index=[date])
+
+    # Save DataFrame to storage
     storage.create(data=df, name=table_name)
+
     return df
```

### Comparing `spai-2024.4.11.post5/spai/project/bck/InstallReqs 2.py` & `spai-2024.4.15/spai/project/bck/InstallReqs 2.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/bck/InstallReqs 3.py` & `spai-2024.4.15/spai/project/bck/InstallReqs 3.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/bck/main.py` & `spai-2024.4.15/spai/project/bck/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/deploy_folder.py` & `spai-2024.4.15/spai/project/deploy_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,12 @@
     # send to api for deployment
     repo = APIRepo()
     data, error = repo.deploy_folder(user, zip_path, variables)
     # clean up
     shutil.rmtree(dst_path)
     if data:
         typer.echo(
-            # f"Check status at {os.getenv('SPAI_UI_URL', 'https://spai.earthpulse.ai')}/dashboard/{data}"
-            f"Check status at {os.getenv('SPAI_UI_URL', 'https://spai.earthpulse.ai')}/dashboard/{data['project_id']}"
+            # f"Check status at {os.getenv('SPAI_UI_URL', 'https://spai.earthpulse.ai')}/my-projects/{data}"
+            f"Check status at {os.getenv('SPAI_UI_URL', 'https://spai.earthpulse.ai')}/my-projects/{data['project_id']}"
         )
         return
     raise Exception(f"Error: {error}")
```

### Comparing `spai-2024.4.11.post5/spai/project/download_template.py` & `spai-2024.4.15/spai/project/download_template.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/get_services.py` & `spai-2024.4.15/spai/project/get_services.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/init_project.py` & `spai-2024.4.15/spai/project/init_project.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/install_requirements.py` & `spai-2024.4.15/spai/project/install_requirements.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/project-template/README.md` & `spai-2024.4.15/spai/project/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/project-template/apis/analytics/main.py` & `spai-2024.4.15/spai/project/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/project-template/apis/xyz/main.py` & `spai-2024.4.15/spai/project/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/project-template/notebooks/analytics/main.ipynb` & `spai-2024.4.15/spai/project/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/project-template/scripts/analytics/main.py` & `spai-2024.4.15/spai/project/project-template/scripts/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/project-template/scripts/downloader/main.py` & `spai-2024.4.15/spai/project/project-template/scripts/downloader/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/project-template/spai.config.yaml` & `spai-2024.4.15/spai/project/project-template/spai.config.yaml`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/project-template/uis/map/main.py` & `spai-2024.4.15/spai/project/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/run_local.py` & `spai-2024.4.15/spai/project/run_local.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/project/stop_service.py` & `spai-2024.4.15/spai/project/stop_service.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/reports/generate.py` & `spai-2024.4.15/spai/reports/generate.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/repos/APIRepo.py` & `spai-2024.4.15/spai/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/repos/AuthRepo.py` & `spai-2024.4.15/spai/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/storage/BaseStorage.py` & `spai-2024.4.15/spai/storage/BaseStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,28 +32,28 @@
             # if ext == "csv":
             #     return self.create_from_csv(data, name)
             # elif ext == "json":
             #     return self.create_from_json(data, name)
             # else:
             #     raise TypeError("Not a valid dataframe type")
         elif isinstance(data, dict):
-            print("hola")
             return self.create_from_dict(data, name)
         elif hasattr(data, "variables") and hasattr(data, "coords"):
             # Object is like a xr.Dataset
             return self.create_from_xarray(data, name)
         else:
             raise TypeError("Not a valid type")
 
     def create_from_data(self, data, path):
         with open(path, "wb") as f:
             f.write(data.read())
         return path
 
     def read(self, name):
+        print("hola")
         ext = name.split(".")[-1]
         if ext == "npy":
             return self.read_from_array(name)
         elif ext in ["tif", "tiff"]:
             return self.read_from_rasterio(name)
         elif ext == "csv":
             return self.read_from_csv(name)
```

### Comparing `spai-2024.4.11.post5/spai/storage/CloudStorage.py` & `spai-2024.4.15/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/storage/LocalStorage.py` & `spai-2024.4.15/spai/storage/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/storage/S3Storage.py` & `spai-2024.4.15/spai/storage/S3Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/storage/Storage.py` & `spai-2024.4.15/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/storage/_S3Storage.py` & `spai-2024.4.15/spai/storage/_S3Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/storage/decorators.py` & `spai-2024.4.15/spai/storage/decorators.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/spai/storage/minio.py` & `spai-2024.4.15/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2024.4.11.post5/PKG-INFO` & `spai-2024.4.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spai
-Version: 2024.4.11.post5
+Version: 2024.4.15
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

