# Comparing `tmp/DLMS_Firmware_updater-0.2.0.tar.gz` & `tmp/DLMS_Firmware_updater-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_Firmware_updater-0.2.0.tar", last modified: Fri Apr 12 13:20:16 2024, max compression
+gzip compressed data, was "DLMS_Firmware_updater-0.2.1.tar", last modified: Mon Apr 15 10:30:30 2024, max compression
```

## Comparing `DLMS_Firmware_updater-0.2.0.tar` & `DLMS_Firmware_updater-0.2.1.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.234088 DLMS_Firmware_updater-0.2.0/
--rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      569 2024-04-12 13:20:16.234088 DLMS_Firmware_updater-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.2.0/README.md
--rw-rw-rw-   0        0        0     1115 2024-04-12 13:00:21.000000 DLMS_Firmware_updater-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 13:20:16.235089 DLMS_Firmware_updater-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.898094 DLMS_Firmware_updater-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.923095 DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/__init__.py
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/config.toml
--rw-rw-rw-   0        0        0     3612 2024-04-12 13:09:16.000000 DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/main.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.938092 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/
--rw-rw-rw-   0        0        0      569 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5345 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.946094 DLMS_Firmware_updater-0.2.0/test/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.949094 DLMS_Firmware_updater-0.2.0/test/Firmwares/
--rw-rw-rw-   0        0        0  1766884 2024-02-16 08:53:58.000000 DLMS_Firmware_updater-0.2.0/test/Firmwares/firmwares.dat
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.905098 DLMS_Firmware_updater-0.2.0/test/Types/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.900095 DLMS_Firmware_updater-0.2.0/test/Types/101/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.004092 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/
--rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.14.typ
--rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.16.typ
--rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.26.typ
--rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.39.typ
--rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.43.typ
--rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.45.typ
--rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.46.typ
--rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.48.typ
--rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.49.typ
--rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.53.typ
--rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.54.typ
--rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.1.0.typ
--rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.2.0.typ
--rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.0.typ
--rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.30.typ
--rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.7.typ
--rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.9.typ
--rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.4.0.typ
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.901094 DLMS_Firmware_updater-0.2.0/test/Types/102/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.049091 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/
--rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.20.typ
--rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.26.typ
--rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.39.typ
--rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.41.typ
--rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.43.typ
--rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.45.typ
--rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.48.typ
--rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.49.typ
--rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.53.typ
--rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.1.0.typ
--rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.2.0.typ
--rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.0.typ
--rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.30.typ
--rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.5.typ
--rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.7.typ
--rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.903093 DLMS_Firmware_updater-0.2.0/test/Types/103/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.088091 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/
--rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.16.typ
--rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.26.typ
--rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.39.typ
--rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.43.typ
--rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.45.typ
--rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.48.typ
--rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.49.typ
--rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.1.0.typ
--rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.2.0.typ
--rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.0.typ
--rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.30.typ
--rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.7.typ
--rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.904094 DLMS_Firmware_updater-0.2.0/test/Types/104/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.123090 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/
--rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.20.typ
--rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.26.typ
--rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.39.typ
--rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.43.typ
--rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.45.typ
--rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.48.typ
--rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.49.typ
--rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.1.0.typ
--rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.2.0.typ
--rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.0.typ
--rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.30.typ
--rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.7.typ
--rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.126092 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.150091 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.0.typ
--rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.15.typ
--rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.16.typ
--rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.17.typ
--rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.0.typ
--rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.3.typ
--rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.7.typ
--rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.6.1.typ
--rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.174090 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.0.typ
--rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.10.typ
--rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.12.typ
--rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.15.typ
--rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.16.typ
--rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.17.typ
--rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.5.0.typ
--rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.5.7.typ
--rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.192089 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
--rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
--rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
--rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
--rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
--rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
--rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.211090 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
--rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
--rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
--rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
--rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
--rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
--rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.231089 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
--rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
--rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
--rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
--rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
--rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
--rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
--rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/image_transfer_1.typ
--rw-rw-rw-   0        0        0    35431 2024-04-12 13:19:19.000000 DLMS_Firmware_updater-0.2.0/test/client_log.txt
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.2.0/test/config.toml
--rw-rw-rw-   0        0        0      387 2024-04-12 13:11:37.000000 DLMS_Firmware_updater-0.2.0/test/test_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.710527 DLMS_Firmware_updater-0.2.1/
+-rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      569 2024-04-15 10:30:30.709525 DLMS_Firmware_updater-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1115 2024-04-15 10:27:37.000000 DLMS_Firmware_updater-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 10:30:30.710527 DLMS_Firmware_updater-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.294226 DLMS_Firmware_updater-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.371525 DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/__init__.py
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/config.toml
+-rw-rw-rw-   0        0        0     3612 2024-04-12 13:09:16.000000 DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/main.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.401531 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/
+-rw-rw-rw-   0        0        0      569 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5345 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.417531 DLMS_Firmware_updater-0.2.1/test/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.422525 DLMS_Firmware_updater-0.2.1/test/Firmwares/
+-rw-rw-rw-   0        0        0  1766884 2024-02-16 08:53:58.000000 DLMS_Firmware_updater-0.2.1/test/Firmwares/firmwares.dat
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.302269 DLMS_Firmware_updater-0.2.1/test/Types/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.297223 DLMS_Firmware_updater-0.2.1/test/Types/101/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.489528 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/
+-rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.14.typ
+-rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.16.typ
+-rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.26.typ
+-rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.39.typ
+-rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.43.typ
+-rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.45.typ
+-rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.46.typ
+-rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.48.typ
+-rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.49.typ
+-rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.53.typ
+-rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.54.typ
+-rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.1.0.typ
+-rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.2.0.typ
+-rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.0.typ
+-rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.30.typ
+-rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.7.typ
+-rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.9.typ
+-rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.4.0.typ
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.299226 DLMS_Firmware_updater-0.2.1/test/Types/102/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.530527 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/
+-rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.20.typ
+-rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.26.typ
+-rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.39.typ
+-rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.41.typ
+-rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.43.typ
+-rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.45.typ
+-rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.48.typ
+-rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.49.typ
+-rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.53.typ
+-rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.1.0.typ
+-rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.2.0.typ
+-rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.0.typ
+-rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.30.typ
+-rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.5.typ
+-rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.7.typ
+-rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.300277 DLMS_Firmware_updater-0.2.1/test/Types/103/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.566527 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/
+-rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.16.typ
+-rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.26.typ
+-rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.39.typ
+-rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.43.typ
+-rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.45.typ
+-rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.48.typ
+-rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.49.typ
+-rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.1.0.typ
+-rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.2.0.typ
+-rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.0.typ
+-rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.30.typ
+-rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.7.typ
+-rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.301256 DLMS_Firmware_updater-0.2.1/test/Types/104/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.601526 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/
+-rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.20.typ
+-rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.26.typ
+-rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.39.typ
+-rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.43.typ
+-rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.45.typ
+-rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.48.typ
+-rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.49.typ
+-rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.1.0.typ
+-rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.2.0.typ
+-rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.0.typ
+-rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.30.typ
+-rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.7.typ
+-rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.604527 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.626563 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.0.typ
+-rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.15.typ
+-rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.16.typ
+-rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.17.typ
+-rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.0.typ
+-rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.3.typ
+-rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.7.typ
+-rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.6.1.typ
+-rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.650537 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.0.typ
+-rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.10.typ
+-rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.12.typ
+-rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.15.typ
+-rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.16.typ
+-rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.17.typ
+-rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.5.0.typ
+-rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.5.7.typ
+-rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.668526 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
+-rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
+-rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
+-rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
+-rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
+-rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
+-rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.687526 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
+-rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
+-rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
+-rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
+-rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
+-rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
+-rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.707527 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
+-rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
+-rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
+-rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
+-rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
+-rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
+-rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
+-rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/image_transfer_1.typ
+-rw-rw-rw-   0        0        0   762665 2024-04-12 13:31:06.000000 DLMS_Firmware_updater-0.2.1/test/client_log.txt
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.2.1/test/config.toml
+-rw-rw-rw-   0        0        0      387 2024-04-12 13:11:37.000000 DLMS_Firmware_updater-0.2.1/test/test_updater.py
```

### Comparing `DLMS_Firmware_updater-0.2.0/PKG-INFO` & `DLMS_Firmware_updater-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_Firmware_updater
-Version: 0.2.0
+Version: 0.2.1
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.2.0/pyproject.toml` & `DLMS_Firmware_updater-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 [tool.setuptools.package-data]
 DLMSFirmwareUpdater = ["*.toml", "*.dat", "*.typ"]
 #exclude = ["test*", "dummy"]  # alternatively: `exclude = ["additional*"]`
 #namespaces = false
 
 [project]
 name = "DLMS_Firmware_updater"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
-    "DLMS_SPODES_client == 0.7.6",
+    "DLMS_SPODES_client == 0.7.8",
     "pyinstaller >= 6.2",
     "build >= 1.2.1"
 ]
 description="dlms-spodes"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords=["dlms", "spodes", "client", "firmware", "update"]
```

### Comparing `DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/config.toml` & `DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/config.toml`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/main.py` & `DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/main.py`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/PKG-INFO` & `DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-Firmware-updater
-Version: 0.2.0
+Version: 0.2.1
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/SOURCES.txt` & `DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Firmwares/firmwares.dat` & `DLMS_Firmware_updater-0.2.1/test/Firmwares/firmwares.dat`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.14.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.14.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.16.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.26.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.39.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.43.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.45.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.46.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.46.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.48.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.49.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.53.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.54.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.54.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.1.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.1.9.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.2.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.2.5.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.30.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.7.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.9.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.20.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.26.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.39.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.41.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.41.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.43.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.45.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.48.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.49.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.53.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.1.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.1.9.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.2.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.2.5.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.30.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.5.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.7.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.9.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.16.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.26.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.39.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.43.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.45.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.48.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.49.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.53.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.1.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.1.9.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.2.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.2.5.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.30.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.7.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.9.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.20.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.26.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.39.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.43.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.45.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.48.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.49.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.53.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.1.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.1.9.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.2.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.2.5.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.30.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.7.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.9.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.15.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.16.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.17.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.22.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.3.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.3.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.7.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.6.1.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.6.1.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.6.2.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.10.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.10.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.12.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.15.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.16.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.17.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.22.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.5.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.5.7.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.6.2.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.15.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.16.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.17.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.22.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.5.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.5.7.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.6.2.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.15.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.16.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.17.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.22.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.5.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.5.7.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.6.2.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.12.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.15.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.16.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.17.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.22.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.5.0.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.5.7.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.6.2.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/image_transfer_1.typ` & `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/image_transfer_1.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.0/test/config.toml` & `DLMS_Firmware_updater-0.2.1/test/config.toml`

 * *Files identical despite different names*

