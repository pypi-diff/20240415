# Comparing `tmp/cbpi4-4.3.2.tar.gz` & `tmp/cbpi4-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-4.3.2.tar", last modified: Fri Feb 23 14:37:04 2024, max compression
+gzip compressed data, was "cbpi4-4.4.0.tar", last modified: Mon Apr 15 05:14:24 2024, max compression
```

## Comparing `cbpi4-4.3.2.tar` & `cbpi4-4.4.0.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:04.242163 cbpi4-4.3.2/
--rw-rw-rw-   0        0        0    35823 2021-12-30 07:59:04.000000 cbpi4-4.3.2/LICENSE
--rw-rw-rw-   0        0        0      100 2021-12-30 07:59:04.000000 cbpi4-4.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2770 2024-02-23 14:37:04.240163 cbpi4-4.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2345 2023-03-10 14:45:36.000000 cbpi4-4.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.400275 cbpi4-4.3.2/cbpi/
--rw-rw-rw-   0        0        0       56 2024-02-23 14:34:33.000000 cbpi4-4.3.2/cbpi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.489277 cbpi4-4.3.2/cbpi/api/
--rw-rw-rw-   0        0        0      841 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/api/__init__.py
--rw-rw-rw-   0        0        0     2248 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/api/actor.py
--rw-rw-rw-   0        0        0     2678 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/api/base.py
--rw-rw-rw-   0        0        0      238 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/api/config.py
--rw-rw-rw-   0        0        0     6738 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/api/dataclasses.py
--rw-rw-rw-   0        0        0     2384 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/api/decorator.py
--rw-rw-rw-   0        0        0      356 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/api/exceptions.py
--rw-rw-rw-   0        0        0     1194 2022-05-09 15:06:48.000000 cbpi4-4.3.2/cbpi/api/extension.py
--rw-rw-rw-   0        0        0     1071 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/api/fermenter_logic.py
--rw-rw-rw-   0        0        0     1068 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/api/kettle_logic.py
--rw-rw-rw-   0        0        0     3821 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/api/property.py
--rw-rw-rw-   0        0        0     1847 2023-03-08 17:51:54.000000 cbpi4-4.3.2/cbpi/api/sensor.py
--rw-rw-rw-   0        0        0     5926 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/api/step.py
--rw-rw-rw-   0        0        0     2508 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/api/timer.py
--rw-rw-rw-   0        0        0    15676 2024-01-12 14:58:31.000000 cbpi4-4.3.2/cbpi/cli.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.612274 cbpi4-4.3.2/cbpi/config/
--rw-rw-rw-   0        0        0       35 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/config/actor.json
--rw-rw-rw-   0        0        0      264 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/config/chromium.desktop
--rw-rw-rw-   0        0        0      844 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/config/config.json
--rw-rw-rw-   0        0        0      262 2023-11-14 17:29:13.000000 cbpi4-4.3.2/cbpi/config/config.yaml
--rw-rw-rw-   0        0        0      151 2023-11-01 13:15:02.000000 cbpi4-4.3.2/cbpi/config/craftbeerpi.template
--rw-rw-rw-   0        0        0     1676 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/config/craftbeerpiboot
--rw-rw-rw-   0        0        0     2711 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/config/create_database.sql
--rw-rw-rw-   0        0        0       35 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/config/fermenter_data.json
--rw-rw-rw-   0        0        0       35 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/config/kettle.json
--rw-rw-rw-   0        0        0       73 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/config/plugin_list.txt
--rw-rw-rw-   0        0        0       36 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/config/sensor.json
--rw-rw-rw-   0        0        0  2029331 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/config/splash.png
--rw-rw-rw-   0        0        0       81 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/config/step_data.json
--rw-rw-rw-   0        0        0    12038 2024-01-20 10:15:45.000000 cbpi4-4.3.2/cbpi/configFolder.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.655277 cbpi4-4.3.2/cbpi/controller/
--rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/controller/__init__.py
--rw-rw-rw-   0        0        0     3418 2022-11-17 18:47:01.000000 cbpi4-4.3.2/cbpi/controller/actor_controller.py
--rw-rw-rw-   0        0        0     7060 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/controller/basic_controller2.py
--rw-rw-rw-   0        0        0     4075 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/controller/config_controller.py
--rw-rw-rw-   0        0        0     3095 2023-11-18 07:09:20.000000 cbpi4-4.3.2/cbpi/controller/dashboard_controller.py
--rw-rw-rw-   0        0        0    24156 2024-02-23 05:45:02.000000 cbpi4-4.3.2/cbpi/controller/fermentation_controller.py
--rw-rw-rw-   0        0        0     2807 2022-05-09 15:06:48.000000 cbpi4-4.3.2/cbpi/controller/fermenter_recipe_controller.py
--rw-rw-rw-   0        0        0     1662 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/controller/job_controller.py
--rw-rw-rw-   0        0        0     1722 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/controller/kettle_controller.py
--rw-rw-rw-   0        0        0     7477 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/controller/log_file_controller.py
--rw-rw-rw-   0        0        0     3336 2023-01-22 15:30:15.000000 cbpi4-4.3.2/cbpi/controller/notification_controller.py
--rw-rw-rw-   0        0        0    10861 2024-01-12 16:34:32.000000 cbpi4-4.3.2/cbpi/controller/plugin_controller.py
--rw-rw-rw-   0        0        0     2849 2022-05-09 15:06:48.000000 cbpi4-4.3.2/cbpi/controller/recipe_controller.py
--rw-rw-rw-   0        0        0     8187 2024-02-23 14:33:58.000000 cbpi4-4.3.2/cbpi/controller/satellite_controller.py
--rw-rw-rw-   0        0        0     1040 2023-03-08 18:10:16.000000 cbpi4-4.3.2/cbpi/controller/sensor_controller.py
--rw-rw-rw-   0        0        0    13721 2024-01-13 14:17:35.000000 cbpi4-4.3.2/cbpi/controller/step_controller.py
--rw-rw-rw-   0        0        0    13935 2024-01-13 10:53:53.000000 cbpi4-4.3.2/cbpi/controller/system_controller.py
--rw-rw-rw-   0        0        0    54604 2023-09-08 16:04:55.000000 cbpi4-4.3.2/cbpi/controller/upload_controller.py
--rw-rw-rw-   0        0        0    13265 2024-01-20 14:52:09.000000 cbpi4-4.3.2/cbpi/craftbeerpi.py
--rw-rw-rw-   0        0        0     7029 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/eventbus.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.658271 cbpi4-4.3.2/cbpi/extension/
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.671273 cbpi4-4.3.2/cbpi/extension/ConfigUpdate/
--rw-rw-rw-   0        0        0    34272 2023-11-18 07:05:48.000000 cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.709271 cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__pycache__/
--rw-rw-rw-   0        0        0     8582 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    32616 2024-01-20 19:31:32.000000 cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     7583 2022-02-16 16:13:43.000000 cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0    12250 2023-11-18 07:13:46.000000 cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       47 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/ConfigUpdate/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.721274 cbpi4-4.3.2/cbpi/extension/FermentationStep/
--rw-rw-rw-   0        0        0    20143 2022-05-09 15:06:48.000000 cbpi4-4.3.2/cbpi/extension/FermentationStep/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.761271 cbpi4-4.3.2/cbpi/extension/FermentationStep/__pycache__/
--rw-rw-rw-   0        0        0    14091 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    34360 2023-01-15 12:43:43.000000 cbpi4-4.3.2/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    11626 2022-02-25 13:23:11.000000 cbpi4-4.3.2/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0    14328 2022-05-09 15:22:15.000000 cbpi4-4.3.2/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       48 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/extension/FermentationStep/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.773276 cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/
--rw-rw-rw-   0        0        0    12986 2024-01-13 15:29:15.000000 cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.825276 cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__pycache__/
--rw-rw-rw-   0        0        0     7807 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    18493 2024-01-20 19:31:33.000000 cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     4843 2022-01-03 11:51:56.000000 cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     8520 2024-01-20 10:16:06.000000 cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       51 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.846278 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_CSV/
--rw-rw-rw-   0        0        0     2359 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_CSV/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.874275 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_CSV/__pycache__/
--rw-rw-rw-   0        0        0     3871 2023-11-01 13:42:14.000000 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_CSV/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2154 2023-05-17 17:58:51.000000 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_CSV/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       52 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_CSV/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.890803 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_InfluxDB/
--rw-rw-rw-   0        0        0     4956 2023-06-29 17:14:15.000000 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_InfluxDB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.917465 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/
--rw-rw-rw-   0        0        0     7530 2023-11-01 13:42:14.000000 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3618 2023-08-04 15:39:37.000000 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       57 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/extension/SensorLogTarget_InfluxDB/config.yaml
--rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.959464 cbpi4-4.3.2/cbpi/extension/__pycache__/
--rw-rw-rw-   0        0        0      130 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      146 2023-01-15 12:43:43.000000 cbpi4-4.3.2/cbpi/extension/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      155 2021-12-30 07:59:45.000000 cbpi4-4.3.2/cbpi/extension/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      159 2022-02-26 13:38:02.000000 cbpi4-4.3.2/cbpi/extension/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.971469 cbpi4-4.3.2/cbpi/extension/dummyactor/
--rw-rw-rw-   0        0        0     1281 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/dummyactor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.016465 cbpi4-4.3.2/cbpi/extension/dummyactor/__pycache__/
--rw-rw-rw-   0        0        0     2167 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/dummyactor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3282 2023-01-15 12:43:43.000000 cbpi4-4.3.2/cbpi/extension/dummyactor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2181 2021-12-30 07:59:45.000000 cbpi4-4.3.2/cbpi/extension/dummyactor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     2202 2022-02-26 13:38:02.000000 cbpi4-4.3.2/cbpi/extension/dummyactor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       42 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/dummyactor/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.030467 cbpi4-4.3.2/cbpi/extension/dummysensor/
--rw-rw-rw-   0        0        0     2728 2023-03-07 19:37:46.000000 cbpi4-4.3.2/cbpi/extension/dummysensor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.075464 cbpi4-4.3.2/cbpi/extension/dummysensor/__pycache__/
--rw-rw-rw-   0        0        0     2871 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/dummysensor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     5500 2023-03-09 06:14:16.000000 cbpi4-4.3.2/cbpi/extension/dummysensor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1359 2021-12-30 07:59:45.000000 cbpi4-4.3.2/cbpi/extension/dummysensor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     2971 2023-03-07 19:55:17.000000 cbpi4-4.3.2/cbpi/extension/dummysensor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/dummysensor/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.091478 cbpi4-4.3.2/cbpi/extension/gpioactor/
--rw-rw-rw-   0        0        0     6111 2023-03-10 17:08:18.000000 cbpi4-4.3.2/cbpi/extension/gpioactor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.134467 cbpi4-4.3.2/cbpi/extension/gpioactor/__pycache__/
--rw-rw-rw-   0        0        0     5776 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/gpioactor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    11052 2023-04-08 13:23:29.000000 cbpi4-4.3.2/cbpi/extension/gpioactor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     5823 2022-02-16 16:13:43.000000 cbpi4-4.3.2/cbpi/extension/gpioactor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     5737 2023-03-10 17:08:23.000000 cbpi4-4.3.2/cbpi/extension/gpioactor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       41 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/gpioactor/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.141464 cbpi4-4.3.2/cbpi/extension/httpsensor/
--rw-rw-rw-   0        0        0     7781 2023-03-28 04:58:15.000000 cbpi4-4.3.2/cbpi/extension/httpsensor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.191465 cbpi4-4.3.2/cbpi/extension/httpsensor/__pycache__/
--rw-rw-rw-   0        0        0     3249 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/httpsensor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    11520 2023-04-08 13:23:29.000000 cbpi4-4.3.2/cbpi/extension/httpsensor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3212 2021-12-30 07:59:45.000000 cbpi4-4.3.2/cbpi/extension/httpsensor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     6177 2023-03-31 15:24:45.000000 cbpi4-4.3.2/cbpi/extension/httpsensor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/httpsensor/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.205464 cbpi4-4.3.2/cbpi/extension/hysteresis/
--rw-rw-rw-   0        0        0     2210 2023-03-02 05:51:03.000000 cbpi4-4.3.2/cbpi/extension/hysteresis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.246465 cbpi4-4.3.2/cbpi/extension/hysteresis/__pycache__/
--rw-rw-rw-   0        0        0     1905 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/hysteresis/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4025 2023-03-09 06:14:16.000000 cbpi4-4.3.2/cbpi/extension/hysteresis/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1798 2021-12-30 07:59:45.000000 cbpi4-4.3.2/cbpi/extension/hysteresis/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     2012 2023-03-04 10:48:54.000000 cbpi4-4.3.2/cbpi/extension/hysteresis/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       48 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/hysteresis/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.259464 cbpi4-4.3.2/cbpi/extension/mashstep/
--rw-rw-rw-   0        0        0    26901 2023-02-11 14:27:45.000000 cbpi4-4.3.2/cbpi/extension/mashstep/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.309464 cbpi4-4.3.2/cbpi/extension/mashstep/__pycache__/
--rw-rw-rw-   0        0        0    19082 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/mashstep/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    46297 2023-03-09 06:14:16.000000 cbpi4-4.3.2/cbpi/extension/mashstep/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    20852 2022-01-04 06:30:42.000000 cbpi4-4.3.2/cbpi/extension/mashstep/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0    21087 2023-02-11 14:27:52.000000 cbpi4-4.3.2/cbpi/extension/mashstep/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       40 2022-01-04 06:30:19.000000 cbpi4-4.3.2/cbpi/extension/mashstep/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.330467 cbpi4-4.3.2/cbpi/extension/mqtt_actor/
--rw-rw-rw-   0        0        0      650 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.550632 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/
--rw-rw-rw-   0        0        0      804 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1278 2023-01-15 12:43:43.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      819 2021-12-30 07:59:45.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      837 2022-03-21 11:27:58.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2164 2023-01-07 21:29:06.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-310.pyc
--rw-rw-rw-   0        0        0     3552 2023-01-15 12:43:43.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-311.pyc
--rw-rw-rw-   0        0        0     2148 2021-12-30 07:59:45.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-37.pyc
--rw-rw-rw-   0        0        0     2173 2022-11-27 13:47:03.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-39.pyc
--rw-rw-rw-   0        0        0     2396 2023-01-07 21:29:05.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-310.pyc
--rw-rw-rw-   0        0        0     4334 2023-01-15 12:43:43.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-311.pyc
--rw-rw-rw-   0        0        0     2338 2022-01-25 10:19:18.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-37.pyc
--rw-rw-rw-   0        0        0     2397 2022-11-27 13:47:03.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-39.pyc
--rw-rw-rw-   0        0        0      869 2023-01-07 21:29:06.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-310.pyc
--rw-rw-rw-   0        0        0     1267 2023-01-15 12:43:43.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-311.pyc
--rw-rw-rw-   0        0        0      874 2021-12-30 07:59:45.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-37.pyc
--rw-rw-rw-   0        0        0      902 2022-03-21 11:27:58.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/config.yaml
--rw-rw-rw-   0        0        0     1702 2022-11-17 18:47:01.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/generic_mqtt_actor.py
--rw-rw-rw-   0        0        0     1922 2022-11-17 18:47:01.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/mqtt_actor.py
--rw-rw-rw-   0        0        0      442 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/extension/mqtt_actor/tasmota_mqtt_actor.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.557628 cbpi4-4.3.2/cbpi/extension/mqtt_sensor/
--rw-rw-rw-   0        0        0     7318 2023-03-28 04:55:57.000000 cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.668633 cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__pycache__/
--rw-rw-rw-   0        0        0     2481 2023-01-07 21:29:06.000000 cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    11932 2023-04-08 13:23:29.000000 cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2438 2021-12-30 07:59:45.000000 cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     5702 2023-03-31 15:24:45.000000 cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/mqtt_sensor/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.685629 cbpi4-4.3.2/cbpi/extension/mqtt_util/
--rw-rw-rw-   0        0        0     2774 2024-02-22 18:43:38.000000 cbpi4-4.3.2/cbpi/extension/mqtt_util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.750627 cbpi4-4.3.2/cbpi/extension/mqtt_util/__pycache__/
--rw-rw-rw-   0        0        0     2130 2023-01-07 21:29:06.000000 cbpi4-4.3.2/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4059 2023-01-15 12:43:43.000000 cbpi4-4.3.2/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2117 2022-02-16 16:13:43.000000 cbpi4-4.3.2/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     2336 2024-02-22 18:43:44.000000 cbpi4-4.3.2/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       42 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/extension/mqtt_util/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.755628 cbpi4-4.3.2/cbpi/extension/onewire/
--rw-rw-rw-   0        0        0     7306 2023-11-01 13:15:02.000000 cbpi4-4.3.2/cbpi/extension/onewire/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.799632 cbpi4-4.3.2/cbpi/extension/onewire/__pycache__/
--rw-rw-rw-   0        0        0     3813 2023-01-07 21:29:06.000000 cbpi4-4.3.2/cbpi/extension/onewire/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    12627 2023-11-01 13:42:13.000000 cbpi4-4.3.2/cbpi/extension/onewire/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3737 2022-01-25 10:19:18.000000 cbpi4-4.3.2/cbpi/extension/onewire/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     6137 2023-11-03 06:31:12.000000 cbpi4-4.3.2/cbpi/extension/onewire/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/extension/onewire/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.815629 cbpi4-4.3.2/cbpi/extension/timer/
--rw-rw-rw-   0        0        0     3267 2023-03-08 18:19:14.000000 cbpi4-4.3.2/cbpi/extension/timer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.838627 cbpi4-4.3.2/cbpi/extension/timer/__pycache__/
--rw-rw-rw-   0        0        0     6763 2023-03-09 06:14:17.000000 cbpi4-4.3.2/cbpi/extension/timer/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3644 2023-03-08 18:19:20.000000 cbpi4-4.3.2/cbpi/extension/timer/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       37 2023-03-07 19:56:41.000000 cbpi4-4.3.2/cbpi/extension/timer/config.yaml
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.876628 cbpi4-4.3.2/cbpi/http_endpoints/
--rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/http_endpoints/__init__.py
--rw-rw-rw-   0        0        0     8004 2023-03-04 14:02:12.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_actor.py
--rw-rw-rw-   0        0        0     3947 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_config.py
--rw-rw-rw-   0        0        0     6405 2023-11-18 07:15:46.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_dashboard.py
--rw-rw-rw-   0        0        0    20118 2022-05-09 15:06:48.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_fermentation.py
--rw-rw-rw-   0        0        0     5003 2023-01-22 15:34:10.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_fermenterrecipe.py
--rw-rw-rw-   0        0        0     8170 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_kettle.py
--rw-rw-rw-   0        0        0     7193 2023-05-14 11:21:02.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_log.py
--rw-rw-rw-   0        0        0     1064 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_login.py
--rw-rw-rw-   0        0        0     1162 2023-01-22 15:34:36.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_notification.py
--rw-rw-rw-   0        0        0     3411 2023-05-17 17:58:07.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_plugin.py
--rw-rw-rw-   0        0        0     4699 2023-01-22 15:34:55.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_recipe.py
--rw-rw-rw-   0        0        0     6512 2023-03-08 17:52:22.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_sensor.py
--rw-rw-rw-   0        0        0     7670 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_step.py
--rw-rw-rw-   0        0        0     7938 2023-01-27 11:25:48.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_system.py
--rw-rw-rw-   0        0        0     5561 2022-03-21 11:22:35.000000 cbpi4-4.3.2/cbpi/http_endpoints/http_upload.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:03.886629 cbpi4-4.3.2/cbpi/job/
--rw-rw-rw-   0        0        0      851 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/job/__init__.py
--rw-rw-rw-   0        0        0     4428 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/job/_job.py
--rw-rw-rw-   0        0        0     4681 2022-11-27 09:48:32.000000 cbpi4-4.3.2/cbpi/job/_scheduler.py
--rw-rw-rw-   0        0        0     1252 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/job/aiohttp.py
--rw-rw-rw-   0        0        0     2948 2023-01-07 16:16:24.000000 cbpi4-4.3.2/cbpi/satellite.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:04.185167 cbpi4-4.3.2/cbpi/static/
--rw-rw-rw-   0        0        0     3329 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/beer_icon.svg
--rw-rw-rw-   0        0        0     2512 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/calculator_icon.svg
--rw-rw-rw-   0        0        0     8711 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/cbpi_icon.svg
--rw-rw-rw-   0        0        0      857 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/control_icon.svg
--rw-rw-rw-   0        0        0     2755 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/glass_icon.svg
--rw-rw-rw-   0        0        0     2931 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/grain.svg
--rw-rw-rw-   0        0        0     4158 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/hops_icon.svg
--rw-rw-rw-   0        0        0     3654 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/kettle2_icon.svg
--rw-rw-rw-   0        0        0      509 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/kettle_icon.svg
--rw-rw-rw-   0        0        0     9743 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/led.svg
--rw-rw-rw-   0        0        0     2499 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/liquid_icon.svg
--rw-rw-rw-   0        0        0     5613 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/paddle_icon.svg
--rw-rw-rw-   0        0        0     3040 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/pipe_icon.svg
--rw-rw-rw-   0        0        0     1746 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/sensor_icon.svg
--rw-rw-rw-   0        0        0  2029331 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/splash.png
--rw-rw-rw-   0        0        0     2615 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/svg_icon.svg
--rw-rw-rw-   0        0        0      713 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/tank_icon.svg
--rw-rw-rw-   0        0        0     1834 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/target_temp.svg
--rw-rw-rw-   0        0        0      258 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/test.html
--rw-rw-rw-   0        0        0     1338 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/thermomenter.svg
--rw-rw-rw-   0        0        0     2946 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/static/yeast.svg
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:04.194165 cbpi4-4.3.2/cbpi/utils/
--rw-rw-rw-   0        0        0       32 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/utils/__init__.py
--rw-rw-rw-   0        0        0      663 2023-01-22 15:35:22.000000 cbpi4-4.3.2/cbpi/utils/encoder.py
--rw-rw-rw-   0        0        0      398 2021-12-30 07:59:04.000000 cbpi4-4.3.2/cbpi/utils/utils.py
--rw-rw-rw-   0        0        0     3314 2023-01-07 16:16:17.000000 cbpi4-4.3.2/cbpi/websocket.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:02.458271 cbpi4-4.3.2/cbpi4.egg-info/
--rw-rw-rw-   0        0        0     2770 2024-02-23 14:37:01.000000 cbpi4-4.3.2/cbpi4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9452 2024-02-23 14:37:01.000000 cbpi4-4.3.2/cbpi4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       33 2024-02-23 14:37:01.000000 cbpi4-4.3.2/cbpi4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-02-23 14:37:01.000000 cbpi4-4.3.2/cbpi4.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      468 2024-02-23 14:37:01.000000 cbpi4-4.3.2/cbpi4.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-23 14:37:01.000000 cbpi4-4.3.2/cbpi4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-23 14:37:04.243165 cbpi4-4.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2457 2024-02-23 14:33:58.000000 cbpi4-4.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-23 14:37:04.237162 cbpi4-4.3.2/tests/
--rw-rw-rw-   0        0        0        0 2021-11-08 11:20:02.000000 cbpi4-4.3.2/tests/__init__.py
--rw-rw-rw-   0        0        0      900 2022-11-17 18:47:01.000000 cbpi4-4.3.2/tests/cbpi_config_fixture.py
--rw-rw-rw-   0        0        0     2713 2023-01-15 14:28:19.000000 cbpi4-4.3.2/tests/test_actor.py
--rw-rw-rw-   0        0        0      462 2022-11-17 18:47:01.000000 cbpi4-4.3.2/tests/test_cli.py
--rw-rw-rw-   0        0        0     1047 2023-01-15 14:33:37.000000 cbpi4-4.3.2/tests/test_config.py
--rw-rw-rw-   0        0        0      819 2023-01-15 14:33:47.000000 cbpi4-4.3.2/tests/test_dashboard.py
--rw-rw-rw-   0        0        0      918 2022-05-09 15:06:48.000000 cbpi4-4.3.2/tests/test_gpio.py
--rw-rw-rw-   0        0        0     1034 2023-01-15 14:34:07.000000 cbpi4-4.3.2/tests/test_index.py
--rw-rw-rw-   0        0        0     1402 2023-01-15 14:33:11.000000 cbpi4-4.3.2/tests/test_kettle.py
--rw-rw-rw-   0        0        0     1011 2023-05-17 17:58:07.000000 cbpi4-4.3.2/tests/test_logger.py
--rw-rw-rw-   0        0        0      245 2023-01-15 14:34:26.000000 cbpi4-4.3.2/tests/test_notification_controller.py
--rw-rw-rw-   0        0        0     1002 2023-11-01 13:48:51.000000 cbpi4-4.3.2/tests/test_sensor.py
--rw-rw-rw-   0        0        0     1379 2023-11-01 13:49:15.000000 cbpi4-4.3.2/tests/test_step.py
--rw-rw-rw-   0        0        0      423 2023-11-01 13:49:24.000000 cbpi4-4.3.2/tests/test_system.py
--rw-rw-rw-   0        0        0     1814 2022-05-09 15:06:48.000000 cbpi4-4.3.2/tests/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:24.480168 cbpi4-4.4.0/
+-rw-rw-rw-   0        0        0    35823 2021-12-30 07:59:04.000000 cbpi4-4.4.0/LICENSE
+-rw-rw-rw-   0        0        0      100 2021-12-30 07:59:04.000000 cbpi4-4.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2770 2024-04-15 05:14:24.479165 cbpi4-4.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2345 2023-03-10 14:45:36.000000 cbpi4-4.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.026772 cbpi4-4.4.0/cbpi/
+-rw-rw-rw-   0        0        0       57 2024-04-13 07:12:09.000000 cbpi4-4.4.0/cbpi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.165771 cbpi4-4.4.0/cbpi/api/
+-rw-rw-rw-   0        0        0      841 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/api/__init__.py
+-rw-rw-rw-   0        0        0     2248 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/api/actor.py
+-rw-rw-rw-   0        0        0     2678 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/api/base.py
+-rw-rw-rw-   0        0        0      238 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/api/config.py
+-rw-rw-rw-   0        0        0     6738 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/api/dataclasses.py
+-rw-rw-rw-   0        0        0     2384 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/api/decorator.py
+-rw-rw-rw-   0        0        0      356 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/api/exceptions.py
+-rw-rw-rw-   0        0        0     1194 2022-05-09 15:06:48.000000 cbpi4-4.4.0/cbpi/api/extension.py
+-rw-rw-rw-   0        0        0     1071 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/api/fermenter_logic.py
+-rw-rw-rw-   0        0        0     1068 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/api/kettle_logic.py
+-rw-rw-rw-   0        0        0     3821 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/api/property.py
+-rw-rw-rw-   0        0        0     1847 2023-03-08 17:51:54.000000 cbpi4-4.4.0/cbpi/api/sensor.py
+-rw-rw-rw-   0        0        0     5926 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/api/step.py
+-rw-rw-rw-   0        0        0     2508 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/api/timer.py
+-rw-rw-rw-   0        0        0    15676 2024-01-12 14:58:31.000000 cbpi4-4.4.0/cbpi/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.314765 cbpi4-4.4.0/cbpi/config/
+-rw-rw-rw-   0        0        0       35 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/config/actor.json
+-rw-rw-rw-   0        0        0      264 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/config/chromium.desktop
+-rw-rw-rw-   0        0        0      844 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/config/config.json
+-rw-rw-rw-   0        0        0      262 2023-11-14 17:29:13.000000 cbpi4-4.4.0/cbpi/config/config.yaml
+-rw-rw-rw-   0        0        0      151 2023-11-01 13:15:02.000000 cbpi4-4.4.0/cbpi/config/craftbeerpi.template
+-rw-rw-rw-   0        0        0     1676 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/config/craftbeerpiboot
+-rw-rw-rw-   0        0        0     2711 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/config/create_database.sql
+-rw-rw-rw-   0        0        0       35 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/config/fermenter_data.json
+-rw-rw-rw-   0        0        0       35 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/config/kettle.json
+-rw-rw-rw-   0        0        0       73 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/config/plugin_list.txt
+-rw-rw-rw-   0        0        0       36 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/config/sensor.json
+-rw-rw-rw-   0        0        0  2029331 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/config/splash.png
+-rw-rw-rw-   0        0        0       81 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/config/step_data.json
+-rw-rw-rw-   0        0        0    12038 2024-01-20 10:15:45.000000 cbpi4-4.4.0/cbpi/configFolder.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.362773 cbpi4-4.4.0/cbpi/controller/
+-rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/controller/__init__.py
+-rw-rw-rw-   0        0        0     3418 2022-11-17 18:47:01.000000 cbpi4-4.4.0/cbpi/controller/actor_controller.py
+-rw-rw-rw-   0        0        0     7060 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/controller/basic_controller2.py
+-rw-rw-rw-   0        0        0     4075 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/controller/config_controller.py
+-rw-rw-rw-   0        0        0     3095 2023-11-18 07:09:20.000000 cbpi4-4.4.0/cbpi/controller/dashboard_controller.py
+-rw-rw-rw-   0        0        0    24156 2024-02-23 05:45:02.000000 cbpi4-4.4.0/cbpi/controller/fermentation_controller.py
+-rw-rw-rw-   0        0        0     2807 2022-05-09 15:06:48.000000 cbpi4-4.4.0/cbpi/controller/fermenter_recipe_controller.py
+-rw-rw-rw-   0        0        0     1662 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/controller/job_controller.py
+-rw-rw-rw-   0        0        0     1722 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/controller/kettle_controller.py
+-rw-rw-rw-   0        0        0     7477 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/controller/log_file_controller.py
+-rw-rw-rw-   0        0        0     3336 2023-01-22 15:30:15.000000 cbpi4-4.4.0/cbpi/controller/notification_controller.py
+-rw-rw-rw-   0        0        0    10861 2024-01-12 16:34:32.000000 cbpi4-4.4.0/cbpi/controller/plugin_controller.py
+-rw-rw-rw-   0        0        0     2849 2022-05-09 15:06:48.000000 cbpi4-4.4.0/cbpi/controller/recipe_controller.py
+-rw-rw-rw-   0        0        0     7199 2024-02-27 16:37:25.000000 cbpi4-4.4.0/cbpi/controller/satellite_controller.py
+-rw-rw-rw-   0        0        0     1040 2023-03-08 18:10:16.000000 cbpi4-4.4.0/cbpi/controller/sensor_controller.py
+-rw-rw-rw-   0        0        0    13721 2024-01-13 14:17:35.000000 cbpi4-4.4.0/cbpi/controller/step_controller.py
+-rw-rw-rw-   0        0        0    13935 2024-01-13 10:53:53.000000 cbpi4-4.4.0/cbpi/controller/system_controller.py
+-rw-rw-rw-   0        0        0    54604 2023-09-08 16:04:55.000000 cbpi4-4.4.0/cbpi/controller/upload_controller.py
+-rw-rw-rw-   0        0        0    13262 2024-02-27 16:37:18.000000 cbpi4-4.4.0/cbpi/craftbeerpi.py
+-rw-rw-rw-   0        0        0     7029 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/eventbus.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.364771 cbpi4-4.4.0/cbpi/extension/
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.379433 cbpi4-4.4.0/cbpi/extension/ConfigUpdate/
+-rw-rw-rw-   0        0        0    34272 2023-11-18 07:05:48.000000 cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.424737 cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__pycache__/
+-rw-rw-rw-   0        0        0     8582 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    32616 2024-01-20 19:31:32.000000 cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7583 2022-02-16 16:13:43.000000 cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0    12250 2023-11-18 07:13:46.000000 cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       47 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/ConfigUpdate/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.438742 cbpi4-4.4.0/cbpi/extension/FermentationStep/
+-rw-rw-rw-   0        0        0    20143 2022-05-09 15:06:48.000000 cbpi4-4.4.0/cbpi/extension/FermentationStep/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.491737 cbpi4-4.4.0/cbpi/extension/FermentationStep/__pycache__/
+-rw-rw-rw-   0        0        0    14091 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    34360 2023-01-15 12:43:43.000000 cbpi4-4.4.0/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    11626 2022-02-25 13:23:11.000000 cbpi4-4.4.0/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0    14328 2022-05-09 15:22:15.000000 cbpi4-4.4.0/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       48 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/extension/FermentationStep/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.508738 cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/
+-rw-rw-rw-   0        0        0    12986 2024-01-13 15:29:15.000000 cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.565740 cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__pycache__/
+-rw-rw-rw-   0        0        0     7807 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    18493 2024-01-20 19:31:33.000000 cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4843 2022-01-03 11:51:56.000000 cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     8520 2024-01-20 10:16:06.000000 cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       51 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.587754 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_CSV/
+-rw-rw-rw-   0        0        0     2359 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_CSV/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.624740 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_CSV/__pycache__/
+-rw-rw-rw-   0        0        0     3871 2023-11-01 13:42:14.000000 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_CSV/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2154 2023-05-17 17:58:51.000000 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_CSV/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       52 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_CSV/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.667742 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_InfluxDB/
+-rw-rw-rw-   0        0        0     4956 2023-06-29 17:14:15.000000 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_InfluxDB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.792748 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/
+-rw-rw-rw-   0        0        0     7530 2023-11-01 13:42:14.000000 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3618 2023-08-04 15:39:37.000000 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       57 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/extension/SensorLogTarget_InfluxDB/config.yaml
+-rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.857739 cbpi4-4.4.0/cbpi/extension/__pycache__/
+-rw-rw-rw-   0        0        0      130 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      146 2023-01-15 12:43:43.000000 cbpi4-4.4.0/cbpi/extension/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      155 2021-12-30 07:59:45.000000 cbpi4-4.4.0/cbpi/extension/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      159 2022-02-26 13:38:02.000000 cbpi4-4.4.0/cbpi/extension/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.877741 cbpi4-4.4.0/cbpi/extension/dummyactor/
+-rw-rw-rw-   0        0        0     1281 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/dummyactor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.943518 cbpi4-4.4.0/cbpi/extension/dummyactor/__pycache__/
+-rw-rw-rw-   0        0        0     2167 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/dummyactor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3282 2023-01-15 12:43:43.000000 cbpi4-4.4.0/cbpi/extension/dummyactor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2181 2021-12-30 07:59:45.000000 cbpi4-4.4.0/cbpi/extension/dummyactor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2202 2022-02-26 13:38:02.000000 cbpi4-4.4.0/cbpi/extension/dummyactor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       42 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/dummyactor/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.961529 cbpi4-4.4.0/cbpi/extension/dummysensor/
+-rw-rw-rw-   0        0        0     2728 2023-03-07 19:37:46.000000 cbpi4-4.4.0/cbpi/extension/dummysensor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.028521 cbpi4-4.4.0/cbpi/extension/dummysensor/__pycache__/
+-rw-rw-rw-   0        0        0     2871 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/dummysensor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5500 2023-03-09 06:14:16.000000 cbpi4-4.4.0/cbpi/extension/dummysensor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1359 2021-12-30 07:59:45.000000 cbpi4-4.4.0/cbpi/extension/dummysensor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2971 2023-03-07 19:55:17.000000 cbpi4-4.4.0/cbpi/extension/dummysensor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/dummysensor/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.047519 cbpi4-4.4.0/cbpi/extension/gpioactor/
+-rw-rw-rw-   0        0        0     6807 2024-02-27 16:37:18.000000 cbpi4-4.4.0/cbpi/extension/gpioactor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.120118 cbpi4-4.4.0/cbpi/extension/gpioactor/__pycache__/
+-rw-rw-rw-   0        0        0     5776 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/gpioactor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11052 2023-04-08 13:23:29.000000 cbpi4-4.4.0/cbpi/extension/gpioactor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5823 2022-02-16 16:13:43.000000 cbpi4-4.4.0/cbpi/extension/gpioactor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6025 2024-02-27 19:02:57.000000 cbpi4-4.4.0/cbpi/extension/gpioactor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       41 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/gpioactor/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.129105 cbpi4-4.4.0/cbpi/extension/httpsensor/
+-rw-rw-rw-   0        0        0     7781 2023-03-28 04:58:15.000000 cbpi4-4.4.0/cbpi/extension/httpsensor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.205114 cbpi4-4.4.0/cbpi/extension/httpsensor/__pycache__/
+-rw-rw-rw-   0        0        0     3249 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/httpsensor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11520 2023-04-08 13:23:29.000000 cbpi4-4.4.0/cbpi/extension/httpsensor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3212 2021-12-30 07:59:45.000000 cbpi4-4.4.0/cbpi/extension/httpsensor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6177 2023-03-31 15:24:45.000000 cbpi4-4.4.0/cbpi/extension/httpsensor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/httpsensor/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.220108 cbpi4-4.4.0/cbpi/extension/hysteresis/
+-rw-rw-rw-   0        0        0     2210 2023-03-02 05:51:03.000000 cbpi4-4.4.0/cbpi/extension/hysteresis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.296103 cbpi4-4.4.0/cbpi/extension/hysteresis/__pycache__/
+-rw-rw-rw-   0        0        0     1905 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/hysteresis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4025 2023-03-09 06:14:16.000000 cbpi4-4.4.0/cbpi/extension/hysteresis/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1798 2021-12-30 07:59:45.000000 cbpi4-4.4.0/cbpi/extension/hysteresis/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2012 2023-03-04 10:48:54.000000 cbpi4-4.4.0/cbpi/extension/hysteresis/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       48 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/hysteresis/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.318104 cbpi4-4.4.0/cbpi/extension/mashstep/
+-rw-rw-rw-   0        0        0    26901 2023-02-11 14:27:45.000000 cbpi4-4.4.0/cbpi/extension/mashstep/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.378103 cbpi4-4.4.0/cbpi/extension/mashstep/__pycache__/
+-rw-rw-rw-   0        0        0    19082 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/mashstep/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    46297 2023-03-09 06:14:16.000000 cbpi4-4.4.0/cbpi/extension/mashstep/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    20852 2022-01-04 06:30:42.000000 cbpi4-4.4.0/cbpi/extension/mashstep/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0    21087 2023-02-11 14:27:52.000000 cbpi4-4.4.0/cbpi/extension/mashstep/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       40 2022-01-04 06:30:19.000000 cbpi4-4.4.0/cbpi/extension/mashstep/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.407540 cbpi4-4.4.0/cbpi/extension/mqtt_actor/
+-rw-rw-rw-   0        0        0      650 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.676534 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/
+-rw-rw-rw-   0        0        0      804 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1278 2023-01-15 12:43:43.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      819 2021-12-30 07:59:45.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      837 2022-03-21 11:27:58.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2164 2023-01-07 21:29:06.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3552 2023-01-15 12:43:43.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2148 2021-12-30 07:59:45.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2173 2022-11-27 13:47:03.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2396 2023-01-07 21:29:05.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4334 2023-01-15 12:43:43.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2338 2022-01-25 10:19:18.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2397 2022-11-27 13:47:03.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-39.pyc
+-rw-rw-rw-   0        0        0      869 2023-01-07 21:29:06.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1267 2023-01-15 12:43:43.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-311.pyc
+-rw-rw-rw-   0        0        0      874 2021-12-30 07:59:45.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-37.pyc
+-rw-rw-rw-   0        0        0      902 2022-03-21 11:27:58.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/config.yaml
+-rw-rw-rw-   0        0        0     1702 2022-11-17 18:47:01.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/generic_mqtt_actor.py
+-rw-rw-rw-   0        0        0     1922 2022-11-17 18:47:01.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/mqtt_actor.py
+-rw-rw-rw-   0        0        0      442 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/extension/mqtt_actor/tasmota_mqtt_actor.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.682534 cbpi4-4.4.0/cbpi/extension/mqtt_sensor/
+-rw-rw-rw-   0        0        0     6953 2024-02-27 16:37:25.000000 cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.741539 cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__pycache__/
+-rw-rw-rw-   0        0        0     2481 2023-01-07 21:29:06.000000 cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11932 2023-04-08 13:23:29.000000 cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2438 2021-12-30 07:59:45.000000 cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     5481 2024-02-27 19:02:57.000000 cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/mqtt_sensor/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.762534 cbpi4-4.4.0/cbpi/extension/mqtt_util/
+-rw-rw-rw-   0        0        0     2774 2024-02-22 18:43:38.000000 cbpi4-4.4.0/cbpi/extension/mqtt_util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.855802 cbpi4-4.4.0/cbpi/extension/mqtt_util/__pycache__/
+-rw-rw-rw-   0        0        0     2130 2023-01-07 21:29:06.000000 cbpi4-4.4.0/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4059 2023-01-15 12:43:43.000000 cbpi4-4.4.0/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2117 2022-02-16 16:13:43.000000 cbpi4-4.4.0/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2336 2024-02-22 18:43:44.000000 cbpi4-4.4.0/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       42 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/extension/mqtt_util/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.863704 cbpi4-4.4.0/cbpi/extension/onewire/
+-rw-rw-rw-   0        0        0     7306 2023-11-01 13:15:02.000000 cbpi4-4.4.0/cbpi/extension/onewire/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.931381 cbpi4-4.4.0/cbpi/extension/onewire/__pycache__/
+-rw-rw-rw-   0        0        0     3813 2023-01-07 21:29:06.000000 cbpi4-4.4.0/cbpi/extension/onewire/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12627 2023-11-01 13:42:13.000000 cbpi4-4.4.0/cbpi/extension/onewire/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3737 2022-01-25 10:19:18.000000 cbpi4-4.4.0/cbpi/extension/onewire/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6137 2023-11-03 06:31:12.000000 cbpi4-4.4.0/cbpi/extension/onewire/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       43 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/extension/onewire/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.949762 cbpi4-4.4.0/cbpi/extension/timer/
+-rw-rw-rw-   0        0        0     3267 2023-03-08 18:19:14.000000 cbpi4-4.4.0/cbpi/extension/timer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:23.982987 cbpi4-4.4.0/cbpi/extension/timer/__pycache__/
+-rw-rw-rw-   0        0        0     6763 2023-03-09 06:14:17.000000 cbpi4-4.4.0/cbpi/extension/timer/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3644 2023-03-08 18:19:20.000000 cbpi4-4.4.0/cbpi/extension/timer/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       37 2023-03-07 19:56:41.000000 cbpi4-4.4.0/cbpi/extension/timer/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:24.035004 cbpi4-4.4.0/cbpi/http_endpoints/
+-rw-rw-rw-   0        0        0        0 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/http_endpoints/__init__.py
+-rw-rw-rw-   0        0        0     8004 2023-03-04 14:02:12.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_actor.py
+-rw-rw-rw-   0        0        0     3947 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_config.py
+-rw-rw-rw-   0        0        0     6405 2023-11-18 07:15:46.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_dashboard.py
+-rw-rw-rw-   0        0        0    20118 2022-05-09 15:06:48.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_fermentation.py
+-rw-rw-rw-   0        0        0     5003 2023-01-22 15:34:10.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_fermenterrecipe.py
+-rw-rw-rw-   0        0        0     8170 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_kettle.py
+-rw-rw-rw-   0        0        0     7193 2023-05-14 11:21:02.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_log.py
+-rw-rw-rw-   0        0        0     1064 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_login.py
+-rw-rw-rw-   0        0        0     1162 2023-01-22 15:34:36.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_notification.py
+-rw-rw-rw-   0        0        0     3411 2023-05-17 17:58:07.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_plugin.py
+-rw-rw-rw-   0        0        0     4699 2023-01-22 15:34:55.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_recipe.py
+-rw-rw-rw-   0        0        0     6512 2023-03-08 17:52:22.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_sensor.py
+-rw-rw-rw-   0        0        0     7670 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_step.py
+-rw-rw-rw-   0        0        0     7938 2023-01-27 11:25:48.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_system.py
+-rw-rw-rw-   0        0        0     5561 2022-03-21 11:22:35.000000 cbpi4-4.4.0/cbpi/http_endpoints/http_upload.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:24.051141 cbpi4-4.4.0/cbpi/job/
+-rw-rw-rw-   0        0        0      851 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/job/__init__.py
+-rw-rw-rw-   0        0        0     4428 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/job/_job.py
+-rw-rw-rw-   0        0        0     4681 2022-11-27 09:48:32.000000 cbpi4-4.4.0/cbpi/job/_scheduler.py
+-rw-rw-rw-   0        0        0     1252 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/job/aiohttp.py
+-rw-rw-rw-   0        0        0     2948 2023-01-07 16:16:24.000000 cbpi4-4.4.0/cbpi/satellite.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:24.419163 cbpi4-4.4.0/cbpi/static/
+-rw-rw-rw-   0        0        0     3329 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/beer_icon.svg
+-rw-rw-rw-   0        0        0     2512 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/calculator_icon.svg
+-rw-rw-rw-   0        0        0     8711 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/cbpi_icon.svg
+-rw-rw-rw-   0        0        0      857 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/control_icon.svg
+-rw-rw-rw-   0        0        0     2755 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/glass_icon.svg
+-rw-rw-rw-   0        0        0     2931 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/grain.svg
+-rw-rw-rw-   0        0        0     4158 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/hops_icon.svg
+-rw-rw-rw-   0        0        0     3654 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/kettle2_icon.svg
+-rw-rw-rw-   0        0        0      509 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/kettle_icon.svg
+-rw-rw-rw-   0        0        0     9743 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/led.svg
+-rw-rw-rw-   0        0        0     2499 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/liquid_icon.svg
+-rw-rw-rw-   0        0        0     5613 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/paddle_icon.svg
+-rw-rw-rw-   0        0        0     3040 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/pipe_icon.svg
+-rw-rw-rw-   0        0        0     1746 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/sensor_icon.svg
+-rw-rw-rw-   0        0        0  2029331 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/splash.png
+-rw-rw-rw-   0        0        0     2615 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/svg_icon.svg
+-rw-rw-rw-   0        0        0      713 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/tank_icon.svg
+-rw-rw-rw-   0        0        0     1834 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/target_temp.svg
+-rw-rw-rw-   0        0        0      258 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/test.html
+-rw-rw-rw-   0        0        0     1338 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/thermomenter.svg
+-rw-rw-rw-   0        0        0     2946 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/static/yeast.svg
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:24.429167 cbpi4-4.4.0/cbpi/utils/
+-rw-rw-rw-   0        0        0       32 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/utils/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-01-22 15:35:22.000000 cbpi4-4.4.0/cbpi/utils/encoder.py
+-rw-rw-rw-   0        0        0      398 2021-12-30 07:59:04.000000 cbpi4-4.4.0/cbpi/utils/utils.py
+-rw-rw-rw-   0        0        0     3314 2023-01-07 16:16:17.000000 cbpi4-4.4.0/cbpi/websocket.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:22.123771 cbpi4-4.4.0/cbpi4.egg-info/
+-rw-rw-rw-   0        0        0     2770 2024-04-15 05:14:21.000000 cbpi4-4.4.0/cbpi4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9452 2024-04-15 05:14:21.000000 cbpi4-4.4.0/cbpi4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       33 2024-04-15 05:14:21.000000 cbpi4-4.4.0/cbpi4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-15 05:14:21.000000 cbpi4-4.4.0/cbpi4.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      468 2024-04-15 05:14:21.000000 cbpi4-4.4.0/cbpi4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-15 05:14:21.000000 cbpi4-4.4.0/cbpi4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 05:14:24.481167 cbpi4-4.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2457 2024-04-12 15:28:09.000000 cbpi4-4.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 05:14:24.475185 cbpi4-4.4.0/tests/
+-rw-rw-rw-   0        0        0        0 2021-11-08 11:20:02.000000 cbpi4-4.4.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      900 2022-11-17 18:47:01.000000 cbpi4-4.4.0/tests/cbpi_config_fixture.py
+-rw-rw-rw-   0        0        0     2713 2023-01-15 14:28:19.000000 cbpi4-4.4.0/tests/test_actor.py
+-rw-rw-rw-   0        0        0      462 2022-11-17 18:47:01.000000 cbpi4-4.4.0/tests/test_cli.py
+-rw-rw-rw-   0        0        0     1047 2023-01-15 14:33:37.000000 cbpi4-4.4.0/tests/test_config.py
+-rw-rw-rw-   0        0        0      819 2023-01-15 14:33:47.000000 cbpi4-4.4.0/tests/test_dashboard.py
+-rw-rw-rw-   0        0        0      918 2022-05-09 15:06:48.000000 cbpi4-4.4.0/tests/test_gpio.py
+-rw-rw-rw-   0        0        0     1034 2023-01-15 14:34:07.000000 cbpi4-4.4.0/tests/test_index.py
+-rw-rw-rw-   0        0        0     1402 2023-01-15 14:33:11.000000 cbpi4-4.4.0/tests/test_kettle.py
+-rw-rw-rw-   0        0        0     1011 2023-05-17 17:58:07.000000 cbpi4-4.4.0/tests/test_logger.py
+-rw-rw-rw-   0        0        0      245 2023-01-15 14:34:26.000000 cbpi4-4.4.0/tests/test_notification_controller.py
+-rw-rw-rw-   0        0        0     1002 2023-11-01 13:48:51.000000 cbpi4-4.4.0/tests/test_sensor.py
+-rw-rw-rw-   0        0        0     1379 2023-11-01 13:49:15.000000 cbpi4-4.4.0/tests/test_step.py
+-rw-rw-rw-   0        0        0      423 2023-11-01 13:49:24.000000 cbpi4-4.4.0/tests/test_system.py
+-rw-rw-rw-   0        0        0     1814 2022-05-09 15:06:48.000000 cbpi4-4.4.0/tests/test_ws.py
```

### Comparing `cbpi4-4.3.2/LICENSE` & `cbpi4-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/PKG-INFO` & `cbpi4-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4
-Version: 4.3.2
+Version: 4.4.0
 Summary: CraftBeerPi4 Brewing Software
 Home-page: http://web.craftbeerpi.com
 Author: Manuel Fritsch / Alexander Vollkopf
 Author-email: manuel@craftbeerpi.com
 License: GPLv3
 Project-URL: Documentation, https://openbrewing.gitbook.io/craftbeerpi4_support/
 Platform: UNKNOWN
```

### Comparing `cbpi4-4.3.2/README.md` & `cbpi4-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/__init__.py` & `cbpi4-4.4.0/cbpi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/actor.py` & `cbpi4-4.4.0/cbpi/api/actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/base.py` & `cbpi4-4.4.0/cbpi/api/base.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/dataclasses.py` & `cbpi4-4.4.0/cbpi/api/dataclasses.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/decorator.py` & `cbpi4-4.4.0/cbpi/api/decorator.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/extension.py` & `cbpi4-4.4.0/cbpi/api/extension.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/fermenter_logic.py` & `cbpi4-4.4.0/cbpi/api/fermenter_logic.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/kettle_logic.py` & `cbpi4-4.4.0/cbpi/api/kettle_logic.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/property.py` & `cbpi4-4.4.0/cbpi/api/property.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/sensor.py` & `cbpi4-4.4.0/cbpi/api/sensor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/step.py` & `cbpi4-4.4.0/cbpi/api/step.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/api/timer.py` & `cbpi4-4.4.0/cbpi/api/timer.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/cli.py` & `cbpi4-4.4.0/cbpi/cli.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/config/config.json` & `cbpi4-4.4.0/cbpi/config/config.json`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/config/craftbeerpiboot` & `cbpi4-4.4.0/cbpi/config/craftbeerpiboot`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/config/create_database.sql` & `cbpi4-4.4.0/cbpi/config/create_database.sql`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/config/splash.png` & `cbpi4-4.4.0/cbpi/config/splash.png`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/configFolder.py` & `cbpi4-4.4.0/cbpi/configFolder.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/actor_controller.py` & `cbpi4-4.4.0/cbpi/controller/actor_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/basic_controller2.py` & `cbpi4-4.4.0/cbpi/controller/basic_controller2.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/config_controller.py` & `cbpi4-4.4.0/cbpi/controller/config_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/dashboard_controller.py` & `cbpi4-4.4.0/cbpi/controller/dashboard_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/fermentation_controller.py` & `cbpi4-4.4.0/cbpi/controller/fermentation_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/fermenter_recipe_controller.py` & `cbpi4-4.4.0/cbpi/controller/fermenter_recipe_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/job_controller.py` & `cbpi4-4.4.0/cbpi/controller/job_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/kettle_controller.py` & `cbpi4-4.4.0/cbpi/controller/kettle_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/log_file_controller.py` & `cbpi4-4.4.0/cbpi/controller/log_file_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/notification_controller.py` & `cbpi4-4.4.0/cbpi/controller/notification_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/plugin_controller.py` & `cbpi4-4.4.0/cbpi/controller/plugin_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/recipe_controller.py` & `cbpi4-4.4.0/cbpi/controller/recipe_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/satellite_controller.py` & `cbpi4-4.4.0/cbpi/controller/satellite_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,393 +120,331 @@
 00000770: 2075 7365 726e 616d 653d 7365 6c66 2e75   username=self.u
 00000780: 7365 726e 616d 652c 2070 6173 7377 6f72  sername, passwor
 00000790: 643d 7365 6c66 2e70 6173 7377 6f72 642c  d=self.password,
 000007a0: 2077 696c 6c3d 5769 6c6c 2874 6f70 6963   will=Will(topic
 000007b0: 3d22 6362 7069 2f64 6973 636f 6e6e 6563  ="cbpi/disconnec
 000007c0: 7422 2c20 7061 796c 6f61 643d 2243 4250  t", payload="CBP
 000007d0: 6920 5365 7276 6572 2044 6973 636f 6e6e  i Server Disconn
-000007e0: 6563 7465 6422 292c 636c 6965 6e74 5f69  ected"),client_i
-000007f0: 643d 7365 6c66 2e63 6c69 656e 745f 6964  d=self.client_id
-00000800: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00000810: 6c6f 6f70 203d 2061 7379 6e63 696f 2e67  loop = asyncio.g
-00000820: 6574 5f65 7665 6e74 5f6c 6f6f 7028 290d  et_event_loop().
-00000830: 0a20 2020 2020 2020 2023 2320 4c69 7374  .        ## List
-00000840: 656e 2066 6f72 206d 7174 7420 6d65 7373  en for mqtt mess
-00000850: 6167 6573 2069 6e20 616e 2028 756e 6177  ages in an (unaw
-00000860: 6169 7465 6429 2061 7379 6e63 696f 2074  aited) asyncio t
-00000870: 6173 6b0d 0a20 2020 2020 2020 2074 6173  ask..        tas
-00000880: 6b20 3d20 7365 6c66 2e6c 6f6f 702e 6372  k = self.loop.cr
-00000890: 6561 7465 5f74 6173 6b28 7365 6c66 2e6c  eate_task(self.l
-000008a0: 6973 7465 6e28 2929 0d0a 2020 2020 2020  isten())..      
-000008b0: 2020 2323 2053 6176 6520 6120 7265 6665    ## Save a refe
-000008c0: 7265 6e63 6520 746f 2074 6865 2074 6173  rence to the tas
-000008d0: 6b20 736f 2069 7420 646f 6573 6e27 7420  k so it doesn't 
-000008e0: 6765 7420 6761 7262 6167 6520 636f 6c6c  get garbage coll
-000008f0: 6563 7465 640d 0a20 2020 2020 2020 2073  ected..        s
-00000900: 656c 662e 7461 736b 732e 6164 6428 7461  elf.tasks.add(ta
-00000910: 736b 290d 0a20 2020 2020 2020 2074 6173  sk)..        tas
-00000920: 6b2e 6164 645f 646f 6e65 5f63 616c 6c62  k.add_done_callb
-00000930: 6163 6b28 7365 6c66 2e74 6173 6b73 2e72  ack(self.tasks.r
-00000940: 656d 6f76 6529 0d0a 0d0a 2020 2020 2020  emove)....      
-00000950: 2020 7365 6c66 2e6c 6f67 6765 722e 696e    self.logger.in
-00000960: 666f 2822 4d51 5454 2043 6f6e 6e65 6374  fo("MQTT Connect
-00000970: 6564 2074 6f20 7b7d 3a7b 7d22 2e66 6f72  ed to {}:{}".for
-00000980: 6d61 7428 7365 6c66 2e68 6f73 742c 2073  mat(self.host, s
-00000990: 656c 662e 706f 7274 2929 0d0a 0d0a 2020  elf.port))....  
-000009a0: 2020 6173 796e 6320 6465 6620 6c69 7374    async def list
-000009b0: 656e 2873 656c 6629 3a0d 0a20 2020 2020  en(self):..     
-000009c0: 2020 2077 6869 6c65 2054 7275 653a 0d0a     while True:..
-000009d0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000009e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000009f0: 2020 6173 796e 6320 7769 7468 2073 656c    async with sel
-00000a00: 662e 636c 6965 6e74 2061 7320 636c 6965  f.client as clie
-00000a10: 6e74 3a0d 0a20 2020 2020 2020 2020 2020  nt:..           
-00000a20: 2020 2020 2020 2020 2061 7379 6e63 2077           async w
-00000a30: 6974 6820 636c 6965 6e74 2e6d 6573 7361  ith client.messa
-00000a40: 6765 7328 2920 6173 206d 6573 7361 6765  ges() as message
-00000a50: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000a60: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00000a70: 7420 636c 6965 6e74 2e73 7562 7363 7269  t client.subscri
-00000a80: 6265 2822 2322 290d 0a20 2020 2020 2020  be("#")..       
+000007e0: 6563 7465 6422 292c 6964 656e 7469 6669  ected"),identifi
+000007f0: 6572 3d73 656c 662e 636c 6965 6e74 5f69  er=self.client_i
+00000800: 6429 0d0a 2020 2020 2020 2020 7365 6c66  d)..        self
+00000810: 2e6c 6f6f 7020 3d20 6173 796e 6369 6f2e  .loop = asyncio.
+00000820: 6765 745f 6576 656e 745f 6c6f 6f70 2829  get_event_loop()
+00000830: 0d0a 2020 2020 2020 2020 2323 204c 6973  ..        ## Lis
+00000840: 7465 6e20 666f 7220 6d71 7474 206d 6573  ten for mqtt mes
+00000850: 7361 6765 7320 696e 2061 6e20 2875 6e61  sages in an (una
+00000860: 7761 6974 6564 2920 6173 796e 6369 6f20  waited) asyncio 
+00000870: 7461 736b 0d0a 2020 2020 2020 2020 7461  task..        ta
+00000880: 736b 203d 2073 656c 662e 6c6f 6f70 2e63  sk = self.loop.c
+00000890: 7265 6174 655f 7461 736b 2873 656c 662e  reate_task(self.
+000008a0: 6c69 7374 656e 2829 290d 0a20 2020 2020  listen())..     
+000008b0: 2020 2023 2320 5361 7665 2061 2072 6566     ## Save a ref
+000008c0: 6572 656e 6365 2074 6f20 7468 6520 7461  erence to the ta
+000008d0: 736b 2073 6f20 6974 2064 6f65 736e 2774  sk so it doesn't
+000008e0: 2067 6574 2067 6172 6261 6765 2063 6f6c   get garbage col
+000008f0: 6c65 6374 6564 0d0a 2020 2020 2020 2020  lected..        
+00000900: 7365 6c66 2e74 6173 6b73 2e61 6464 2874  self.tasks.add(t
+00000910: 6173 6b29 0d0a 2020 2020 2020 2020 7461  ask)..        ta
+00000920: 736b 2e61 6464 5f64 6f6e 655f 6361 6c6c  sk.add_done_call
+00000930: 6261 636b 2873 656c 662e 7461 736b 732e  back(self.tasks.
+00000940: 7265 6d6f 7665 290d 0a0d 0a20 2020 2020  remove)....     
+00000950: 2020 2073 656c 662e 6c6f 6767 6572 2e69     self.logger.i
+00000960: 6e66 6f28 224d 5154 5420 436f 6e6e 6563  nfo("MQTT Connec
+00000970: 7465 6420 746f 207b 7d3a 7b7d 222e 666f  ted to {}:{}".fo
+00000980: 726d 6174 2873 656c 662e 686f 7374 2c20  rmat(self.host, 
+00000990: 7365 6c66 2e70 6f72 7429 290d 0a0d 0a20  self.port)).... 
+000009a0: 2020 2061 7379 6e63 2064 6566 206c 6973     async def lis
+000009b0: 7465 6e28 7365 6c66 293a 0d0a 2020 2020  ten(self):..    
+000009c0: 2020 2020 7768 696c 6520 5472 7565 3a0d      while True:.
+000009d0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+000009e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000009f0: 2020 2061 7379 6e63 2077 6974 6820 7365     async with se
+00000a00: 6c66 2e63 6c69 656e 7420 6173 2063 6c69  lf.client as cli
+00000a10: 656e 743a 0d0a 2020 2020 2020 2020 2020  ent:..          
+00000a20: 2020 2020 2020 2020 2020 2020 2020 6177                aw
+00000a30: 6169 7420 636c 6965 6e74 2e73 7562 7363  ait client.subsc
+00000a40: 7269 6265 2822 2322 290d 0a20 2020 2020  ribe("#")..     
+00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a60: 2020 2061 7379 6e63 2066 6f72 206d 6573     async for mes
+00000a70: 7361 6765 2069 6e20 636c 6965 6e74 2e6d  sage in client.m
+00000a80: 6573 7361 6765 733a 0d0a 2020 2020 2020  essages:..      
 00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000aa0: 2061 7379 6e63 2066 6f72 206d 6573 7361   async for messa
-00000ab0: 6765 2069 6e20 6d65 7373 6167 6573 3a0d  ge in messages:.
-00000ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ad0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00000ae0: 2074 6f70 6963 5f66 696c 7465 7220 696e   topic_filter in
-00000af0: 2073 656c 662e 746f 7069 635f 6669 6c74   self.topic_filt
-00000b00: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
+00000aa0: 2020 2020 2020 666f 7220 746f 7069 635f        for topic_
+00000ab0: 6669 6c74 6572 2069 6e20 7365 6c66 2e74  filter in self.t
+00000ac0: 6f70 6963 5f66 696c 7465 7273 3a0d 0a20  opic_filters:.. 
+00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00000af0: 6f70 6963 203d 2074 6f70 6963 5f66 696c  opic = topic_fil
+00000b00: 7465 725b 305d 0d0a 2020 2020 2020 2020  ter[0]..        
 00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b20: 2020 2020 2020 746f 7069 6320 3d20 746f        topic = to
-00000b30: 7069 635f 6669 6c74 6572 5b30 5d0d 0a20  pic_filter[0].. 
-00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b50: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00000b60: 6574 686f 6420 3d20 746f 7069 635f 6669  ethod = topic_fi
-00000b70: 6c74 6572 5b31 5d0d 0a20 2020 2020 2020  lter[1]..       
-00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b90: 2020 2020 2020 2020 2069 6620 6d65 7373           if mess
-00000ba0: 6167 652e 746f 7069 632e 6d61 7463 6865  age.topic.matche
-00000bb0: 7328 746f 7069 6329 3a0d 0a20 2020 2020  s(topic):..     
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00000be0: 7761 6974 2028 6d65 7468 6f64 286d 6573  wait (method(mes
-00000bf0: 7361 6765 2929 0d0a 2020 2020 2020 2020  sage))..        
-00000c00: 2020 2020 6578 6365 7074 2061 7379 6e63      except async
-00000c10: 696f 2e43 616e 6365 6c6c 6564 4572 726f  io.CancelledErro
-00000c20: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00000c30: 2020 2020 2320 4361 6e63 656c 0d0a 2020      # Cancel..  
-00000c40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00000c50: 6c66 2e6c 6f67 6765 722e 7761 726e 696e  lf.logger.warnin
-00000c60: 6728 224d 5154 5420 4c69 7374 656e 696e  g("MQTT Listenin
-00000c70: 6720 4361 6e63 656c 6c65 6422 290d 0a20  g Cancelled").. 
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00000c90: 7265 616b 0d0a 2020 2020 2020 2020 2020  reak..          
-00000ca0: 2020 6578 6365 7074 204d 7174 7445 7272    except MqttErr
-00000cb0: 6f72 2061 7320 653a 0d0a 2020 2020 2020  or as e:..      
-00000cc0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00000cd0: 6f67 6765 722e 6572 726f 7228 224d 5154  ogger.error("MQT
-00000ce0: 5420 4578 6365 7074 696f 6e3a 207b 7d22  T Exception: {}"
-00000cf0: 2e66 6f72 6d61 7428 6529 290d 0a20 2020  .format(e))..   
-00000d00: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00000d10: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-00000d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d30: 2073 656c 662e 6c6f 6767 6572 2e65 7272   self.logger.err
-00000d40: 6f72 2822 4d51 5454 2047 656e 6572 616c  or("MQTT General
-00000d50: 2045 7863 6570 7469 6f6e 3a20 7b7d 222e   Exception: {}".
-00000d60: 666f 726d 6174 2865 2929 0d0a 2020 2020  format(e))..    
-00000d70: 2020 2020 2020 2020 6177 6169 7420 6173          await as
-00000d80: 796e 6369 6f2e 736c 6565 7028 3529 0d0a  yncio.sleep(5)..
-00000d90: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
-00000da0: 6620 7075 626c 6973 6828 7365 6c66 2c20  f publish(self, 
-00000db0: 746f 7069 632c 206d 6573 7361 6765 2c20  topic, message, 
-00000dc0: 7265 7461 696e 3d46 616c 7365 293a 0d0a  retain=False):..
-00000dd0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00000de0: 636c 6965 6e74 2069 7320 6e6f 7420 4e6f  client is not No
-00000df0: 6e65 2061 6e64 2073 656c 662e 636c 6965  ne and self.clie
-00000e00: 6e74 2e5f 636f 6e6e 6563 7465 643a 0d0a  nt._connected:..
-00000e10: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00000e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000e30: 2020 6177 6169 7420 7365 6c66 2e63 6c69    await self.cli
-00000e40: 656e 742e 7075 626c 6973 6828 746f 7069  ent.publish(topi
-00000e50: 632c 206d 6573 7361 6765 2c20 716f 733d  c, message, qos=
-00000e60: 312c 2072 6574 6169 6e3d 7265 7461 696e  1, retain=retain
-00000e70: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00000e80: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00000e90: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
-00000ea0: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
-00000eb0: 6572 2e77 6172 6e69 6e67 2822 4661 696c  er.warning("Fail
-00000ec0: 6564 2074 6f20 7075 7368 2064 6174 6120  ed to push data 
-00000ed0: 7669 6120 6d71 7474 3a20 7b7d 222e 666f  via mqtt: {}".fo
-00000ee0: 726d 6174 2865 2929 0d0a 0d0a 2020 2020  rmat(e))....    
-00000ef0: 6173 796e 6320 6465 6620 5f61 6374 6f72  async def _actor
-00000f00: 5f6f 6e28 7365 6c66 2c20 6d65 7373 6167  _on(self, messag
-00000f10: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00000f20: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00000f30: 2020 2020 2020 2074 6f70 6963 5f6b 6579         topic_key
-00000f40: 203d 2073 7472 286d 6573 7361 6765 2e74   = str(message.t
-00000f50: 6f70 6963 292e 7370 6c69 7428 222f 2229  opic).split("/")
-00000f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000f70: 2020 6177 6169 7420 7365 6c66 2e63 6270    await self.cbp
-00000f80: 692e 6163 746f 722e 6f6e 2874 6f70 6963  i.actor.on(topic
-00000f90: 5f6b 6579 5b32 5d29 0d0a 2020 2020 2020  _key[2])..      
-00000fa0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00000fb0: 6f67 6765 722e 7761 726e 696e 6728 2250  ogger.warning("P
-00000fc0: 726f 6365 7373 6564 2061 6374 6f72 207b  rocessed actor {
-00000fd0: 7d20 6f6e 2076 6961 206d 7174 7422 2e66  } on via mqtt".f
-00000fe0: 6f72 6d61 7428 746f 7069 635f 6b65 795b  ormat(topic_key[
-00000ff0: 325d 2929 0d0a 2020 2020 2020 2020 2020  2]))..          
-00001000: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00001010: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
-00001020: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00001030: 6f67 6765 722e 7761 726e 696e 6728 2246  ogger.warning("F
-00001040: 6169 6c65 6420 746f 2070 726f 6365 7373  ailed to process
-00001050: 2061 6374 6f72 206f 6e20 7669 6120 6d71   actor on via mq
-00001060: 7474 3a20 7b7d 222e 666f 726d 6174 2865  tt: {}".format(e
-00001070: 2929 0d0a 0d0a 2020 2020 6173 796e 6320  ))....    async 
-00001080: 6465 6620 5f61 6374 6f72 5f6f 6666 2873  def _actor_off(s
-00001090: 656c 662c 206d 6573 7361 6765 293a 0d0a  elf, message):..
-000010a0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000010b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000010c0: 2020 746f 7069 635f 6b65 7920 3d20 7374    topic_key = st
-000010d0: 7228 6d65 7373 6167 652e 746f 7069 6329  r(message.topic)
-000010e0: 2e73 706c 6974 2822 2f22 290d 0a20 2020  .split("/")..   
-000010f0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-00001100: 6974 2073 656c 662e 6362 7069 2e61 6374  it self.cbpi.act
-00001110: 6f72 2e6f 6666 2874 6f70 6963 5f6b 6579  or.off(topic_key
-00001120: 5b32 5d29 0d0a 2020 2020 2020 2020 2020  [2])..          
-00001130: 2020 2020 2020 7365 6c66 2e6c 6f67 6765        self.logge
-00001140: 722e 7761 726e 696e 6728 2250 726f 6365  r.warning("Proce
-00001150: 7373 6564 2061 6374 6f72 207b 7d20 6f66  ssed actor {} of
-00001160: 6620 7669 6120 6d71 7474 222e 666f 726d  f via mqtt".form
-00001170: 6174 2874 6f70 6963 5f6b 6579 5b32 5d29  at(topic_key[2])
-00001180: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00001190: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-000011a0: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
-000011b0: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
-000011c0: 6572 2e77 6172 6e69 6e67 2822 4661 696c  er.warning("Fail
-000011d0: 6564 2074 6f20 7072 6f63 6573 7320 6163  ed to process ac
-000011e0: 746f 7220 6f66 6620 7669 6120 6d71 7474  tor off via mqtt
-000011f0: 3a20 7b7d 222e 666f 726d 6174 2865 2929  : {}".format(e))
-00001200: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
-00001210: 6620 5f61 6374 6f72 5f70 6f77 6572 2873  f _actor_power(s
-00001220: 656c 662c 206d 6573 7361 6765 293a 0d0a  elf, message):..
-00001230: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00001240: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001250: 2020 746f 7069 635f 6b65 7920 3d20 7374    topic_key = st
-00001260: 7228 6d65 7373 6167 652e 746f 7069 6329  r(message.topic)
-00001270: 2e73 706c 6974 2822 2f22 290d 0a20 2020  .split("/")..   
-00001280: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00001290: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000012a0: 2020 2020 2020 2070 6f77 6572 3d69 6e74         power=int
-000012b0: 286d 6573 7361 6765 2e70 6179 6c6f 6164  (message.payload
-000012c0: 2e64 6563 6f64 6528 2929 0d0a 2020 2020  .decode())..    
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012e0: 6966 2070 6f77 6572 203e 2031 3030 3a20  if power > 100: 
-000012f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001300: 2020 2020 2020 2020 2020 706f 7765 7220            power 
-00001310: 3d20 3130 300d 0a20 2020 2020 2020 2020  = 100..         
-00001320: 2020 2020 2020 2020 2020 2069 6620 706f             if po
-00001330: 7765 7220 3c20 303a 0d0a 2020 2020 2020  wer < 0:..      
-00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001350: 2020 706f 7765 7220 3d20 300d 0a20 2020    power = 0..   
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2061 7761 6974 2073 656c 662e 6362 7069   await self.cbpi
-00001380: 2e61 6374 6f72 2e73 6574 5f70 6f77 6572  .actor.set_power
-00001390: 2874 6f70 6963 5f6b 6579 5b32 5d2c 706f  (topic_key[2],po
-000013a0: 7765 7229 0d0a 2020 2020 2020 2020 2020  wer)..          
-000013b0: 2020 2020 2020 2020 2020 2361 7761 6974            #await
-000013c0: 2073 656c 662e 6362 7069 2e61 6374 6f72   self.cbpi.actor
-000013d0: 2e61 6374 6f72 5f75 7064 6174 6528 746f  .actor_update(to
-000013e0: 7069 635f 6b65 795b 325d 2c70 6f77 6572  pic_key[2],power
-000013f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001400: 2020 2065 7863 6570 743a 0d0a 2020 2020     except:..    
-00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001420: 7365 6c66 2e6c 6f67 6765 722e 7761 726e  self.logger.warn
-00001430: 696e 6728 2246 6169 6c65 6420 746f 2073  ing("Failed to s
-00001440: 6574 2061 6374 6f72 2070 6f77 6572 2076  et actor power v
-00001450: 6961 206d 7174 742e 204e 6f20 7661 6c69  ia mqtt. No vali
-00001460: 6420 706f 7765 7220 696e 206d 6573 7361  d power in messa
-00001470: 6765 2229 0d0a 2020 2020 2020 2020 2020  ge")..          
-00001480: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
-00001490: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000014a0: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
-000014b0: 4661 696c 6564 2074 6f20 7365 7420 6163  Failed to set ac
-000014c0: 746f 7220 706f 7765 7220 7669 6120 6d71  tor power via mq
-000014d0: 7474 2229 0d0a 0d0a 2020 2020 6173 796e  tt")....    asyn
-000014e0: 6320 6465 6620 5f6b 6574 746c 6575 7064  c def _kettleupd
-000014f0: 6174 6528 7365 6c66 2c20 6d65 7373 6167  ate(self, messag
-00001500: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00001510: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-00001520: 2020 2020 2020 2073 656c 662e 6b65 7474         self.kett
-00001530: 6c65 3d73 656c 662e 6b65 7474 6c65 636f  le=self.kettleco
-00001540: 6e74 726f 6c6c 6572 2e67 6574 5f73 7461  ntroller.get_sta
-00001550: 7465 2829 0d0a 2020 2020 2020 2020 2020  te()..          
-00001560: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
-00001570: 6e20 7365 6c66 2e6b 6574 746c 655b 2764  n self.kettle['d
-00001580: 6174 6127 5d3a 0d0a 2020 2020 2020 2020  ata']:..        
-00001590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000015a0: 2e63 6270 692e 7075 7368 5f75 7064 6174  .cbpi.push_updat
-000015b0: 6528 2263 6270 692f 7b7d 2f7b 7d22 2e66  e("cbpi/{}/{}".f
-000015c0: 6f72 6d61 7428 226b 6574 746c 6575 7064  ormat("kettleupd
-000015d0: 6174 6522 2c69 7465 6d5b 2769 6427 5d29  ate",item['id'])
-000015e0: 2c20 6974 656d 290d 0a20 2020 2020 2020  , item)..       
-000015f0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00001600: 7074 696f 6e20 6173 2065 3a0d 0a20 2020  ption as e:..   
-00001610: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00001620: 662e 6c6f 6767 6572 2e77 6172 6e69 6e67  f.logger.warning
-00001630: 2822 4661 696c 6564 2074 6f20 7365 6e64  ("Failed to send
-00001640: 206b 6574 746c 6575 7064 6174 6520 7669   kettleupdate vi
-00001650: 6120 6d71 7474 3a20 7b7d 222e 666f 726d  a mqtt: {}".form
-00001660: 6174 2865 2929 0d0a 0d0a 2020 2020 6173  at(e))....    as
-00001670: 796e 6320 6465 6620 5f66 6572 6d65 6e74  ync def _ferment
-00001680: 6572 7570 6461 7465 2873 656c 662c 206d  erupdate(self, m
-00001690: 6573 7361 6765 293a 0d0a 2020 2020 2020  essage):..      
-000016a0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-000016b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000016c0: 2e66 6572 6d65 6e74 6572 3d73 656c 662e  .fermenter=self.
-000016d0: 6665 726d 656e 7465 7263 6f6e 7472 6f6c  fermentercontrol
-000016e0: 6c65 722e 6765 745f 7374 6174 6528 290d  ler.get_state().
-000016f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001700: 2066 6f72 2069 7465 6d20 696e 2073 656c   for item in sel
-00001710: 662e 6665 726d 656e 7465 725b 2764 6174  f.fermenter['dat
-00001720: 6127 5d3a 0d0a 2020 2020 2020 2020 2020  a']:..          
-00001730: 2020 2020 2020 2020 2020 6974 656d 5f6e            item_n
-00001740: 6577 3d73 656c 662e 7265 6d6f 7665 5f6b  ew=self.remove_k
-00001750: 6579 2869 7465 6d2c 2273 7465 7073 2229  ey(item,"steps")
-00001760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001770: 2020 2020 2020 7365 6c66 2e63 6270 692e        self.cbpi.
-00001780: 7075 7368 5f75 7064 6174 6528 2263 6270  push_update("cbp
-00001790: 692f 7b7d 2f7b 7d22 2e66 6f72 6d61 7428  i/{}/{}".format(
-000017a0: 2266 6572 6d65 6e74 6572 7570 6461 7465  "fermenterupdate
-000017b0: 222c 6974 656d 5b27 6964 275d 292c 2069  ",item['id']), i
-000017c0: 7465 6d5f 6e65 7729 0d0a 2020 2020 2020  tem_new)..      
-000017d0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-000017e0: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
-000017f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001800: 6c66 2e6c 6f67 6765 722e 7761 726e 696e  lf.logger.warnin
-00001810: 6728 2246 6169 6c65 6420 746f 2073 656e  g("Failed to sen
-00001820: 6420 6665 726d 656e 7465 7275 7064 6174  d fermenterupdat
-00001830: 6520 7669 6120 6d71 7474 3a20 7b7d 222e  e via mqtt: {}".
-00001840: 666f 726d 6174 2865 2929 0d0a 0d0a 2020  format(e))....  
-00001850: 2020 6173 796e 6320 6465 6620 5f61 6374    async def _act
-00001860: 6f72 7570 6461 7465 2873 656c 662c 206d  orupdate(self, m
-00001870: 6573 7361 6765 293a 0d0a 2020 2020 2020  essage):..      
-00001880: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-00001890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000018a0: 2e61 6374 6f72 3d73 656c 662e 6163 746f  .actor=self.acto
-000018b0: 7263 6f6e 7472 6f6c 6c65 722e 6765 745f  rcontroller.get_
-000018c0: 7374 6174 6528 290d 0a20 2020 2020 2020  state()..       
-000018d0: 2020 2020 2020 2020 2066 6f72 2069 7465           for ite
-000018e0: 6d20 696e 2073 656c 662e 6163 746f 725b  m in self.actor[
-000018f0: 2764 6174 6127 5d3a 0d0a 2020 2020 2020  'data']:..      
-00001900: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001910: 6c66 2e63 6270 692e 7075 7368 5f75 7064  lf.cbpi.push_upd
-00001920: 6174 6528 2263 6270 692f 7b7d 2f7b 7d22  ate("cbpi/{}/{}"
-00001930: 2e66 6f72 6d61 7428 2261 6374 6f72 7570  .format("actorup
-00001940: 6461 7465 222c 6974 656d 5b27 6964 275d  date",item['id']
-00001950: 292c 2069 7465 6d29 0d0a 2020 2020 2020  ), item)..      
-00001960: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00001970: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
-00001980: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001990: 6c66 2e6c 6f67 6765 722e 7761 726e 696e  lf.logger.warnin
-000019a0: 6728 2246 6169 6c65 6420 746f 2073 656e  g("Failed to sen
-000019b0: 6420 6163 746f 7275 7064 6174 6520 7669  d actorupdate vi
-000019c0: 6120 6d71 7474 3a20 7b7d 222e 666f 726d  a mqtt: {}".form
-000019d0: 6174 2865 2929 0d0a 0d0a 2020 2020 6173  at(e))....    as
-000019e0: 796e 6320 6465 6620 5f73 656e 736f 7275  ync def _sensoru
-000019f0: 7064 6174 6528 7365 6c66 2c20 6d65 7373  pdate(self, mess
-00001a00: 6167 6529 3a0d 0a20 2020 2020 2020 2020  age):..         
-00001a10: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00001a20: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00001a30: 6e73 6f72 3d73 656c 662e 7365 6e73 6f72  nsor=self.sensor
-00001a40: 636f 6e74 726f 6c6c 6572 2e67 6574 5f73  controller.get_s
-00001a50: 7461 7465 2829 0d0a 2020 2020 2020 2020  tate()..        
-00001a60: 2020 2020 2020 2020 666f 7220 6974 656d          for item
-00001a70: 2069 6e20 7365 6c66 2e73 656e 736f 725b   in self.sensor[
-00001a80: 2764 6174 6127 5d3a 0d0a 2020 2020 2020  'data']:..      
-00001a90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001aa0: 6c66 2e63 6270 692e 7075 7368 5f75 7064  lf.cbpi.push_upd
-00001ab0: 6174 6528 2263 6270 692f 7b7d 2f7b 7d22  ate("cbpi/{}/{}"
-00001ac0: 2e66 6f72 6d61 7428 2273 656e 736f 7275  .format("sensoru
-00001ad0: 7064 6174 6522 2c69 7465 6d5b 2769 6427  pdate",item['id'
-00001ae0: 5d29 2c20 6974 656d 290d 0a20 2020 2020  ]), item)..     
-00001af0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00001b00: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001b20: 656c 662e 6c6f 6767 6572 2e77 6172 6e69  elf.logger.warni
-00001b30: 6e67 2822 4661 696c 6564 2074 6f20 7365  ng("Failed to se
-00001b40: 6e64 2073 656e 736f 7275 7064 6174 6520  nd sensorupdate 
-00001b50: 7669 6120 6d71 7474 3a20 7b7d 222e 666f  via mqtt: {}".fo
-00001b60: 726d 6174 2865 2929 0d0a 0d0a 2020 2020  rmat(e))....    
-00001b70: 6465 6620 7375 6263 7269 6265 2873 656c  def subcribe(sel
-00001b80: 662c 2074 6f70 6963 2c20 6d65 7468 6f64  f, topic, method
-00001b90: 293a 0d0a 2020 2020 2020 2020 7461 736b  ):..        task
-00001ba0: 203d 2061 7379 6e63 696f 2e63 7265 6174   = asyncio.creat
-00001bb0: 655f 7461 736b 2873 656c 662e 5f73 7562  e_task(self._sub
-00001bc0: 6372 6962 6528 746f 7069 632c 206d 6574  cribe(topic, met
-00001bd0: 686f 6429 290d 0a20 2020 2020 2020 2072  hod))..        r
-00001be0: 6574 7572 6e20 7461 736b 0d0a 0d0a 2020  eturn task....  
-00001bf0: 2020 6173 796e 6320 6465 6620 5f73 7562    async def _sub
-00001c00: 6372 6962 6528 7365 6c66 2c20 746f 7069  cribe(self, topi
-00001c10: 632c 206d 6574 686f 6429 3a0d 0a20 2020  c, method):..   
-00001c20: 2020 2020 2073 656c 662e 6572 726f 723d       self.error=
-00001c30: 4661 6c73 650d 0a20 2020 2020 2020 2077  False..        w
-00001c40: 6869 6c65 2054 7275 653a 0d0a 2020 2020  hile True:..    
-00001c50: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00001c60: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001c70: 2073 656c 662e 636c 6965 6e74 2e5f 636f   self.client._co
-00001c80: 6e6e 6563 7465 642e 646f 6e65 2829 3a0d  nnected.done():.
-00001c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ca0: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-00001cb0: 7365 6c66 2e63 6c69 656e 742e 6d65 7373  self.client.mess
-00001cc0: 6167 6573 2829 2061 7320 6d65 7373 6167  ages() as messag
-00001cd0: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-00001ce0: 2020 2020 2020 2020 2020 2020 2061 7761               awa
-00001cf0: 6974 2073 656c 662e 636c 6965 6e74 2e73  it self.client.s
-00001d00: 7562 7363 7269 6265 2874 6f70 6963 290d  ubscribe(topic).
-00001d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d20: 2020 2020 2020 2020 2061 7379 6e63 2066           async f
-00001d30: 6f72 206d 6573 7361 6765 2069 6e20 6d65  or message in me
-00001d40: 7373 6167 6573 3a0d 0a20 2020 2020 2020  ssages:..       
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d60: 2020 2020 2069 6620 6d65 7373 6167 652e       if message.
-00001d70: 746f 7069 632e 6d61 7463 6865 7328 746f  topic.matches(to
-00001d80: 7069 6329 3a0d 0a20 2020 2020 2020 2020  pic):..         
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 2020 2020 2020 2061 7761 6974 206d 6574         await met
-00001db0: 686f 6428 6d65 7373 6167 652e 7061 796c  hod(message.payl
-00001dc0: 6f61 642e 6465 636f 6465 2829 290d 0a20  oad.decode()).. 
-00001dd0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00001de0: 7420 6173 796e 6369 6f2e 4361 6e63 656c  t asyncio.Cancel
-00001df0: 6c65 6445 7272 6f72 3a0d 0a20 2020 2020  ledError:..     
-00001e00: 2020 2020 2020 2020 2020 2023 2043 616e             # Can
-00001e10: 6365 6c0d 0a20 2020 2020 2020 2020 2020  cel..           
-00001e20: 2020 2020 2073 656c 662e 6c6f 6767 6572       self.logger
-00001e30: 2e77 6172 6e69 6e67 2822 5375 6273 6372  .warning("Subscr
-00001e40: 6970 7469 6f6e 207b 7d20 4361 6e63 656c  iption {} Cancel
-00001e50: 6c65 6422 2e66 6f72 6d61 7428 746f 7069  led".format(topi
-00001e60: 6329 290d 0a20 2020 2020 2020 2020 2020  c))..           
-00001e70: 2020 2020 2073 656c 662e 6572 726f 723d       self.error=
-00001e80: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
-00001e90: 2020 6578 6365 7074 204d 7174 7445 7272    except MqttErr
-00001ea0: 6f72 2061 7320 653a 0d0a 2020 2020 2020  or as e:..      
-00001eb0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00001ec0: 6f67 6765 722e 6572 726f 7228 2253 7562  ogger.error("Sub
-00001ed0: 204d 5154 5420 4578 6365 7074 696f 6e3a   MQTT Exception:
-00001ee0: 207b 7d22 2e66 6f72 6d61 7428 6529 290d   {}".format(e)).
-00001ef0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-00001f00: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00001f10: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
-00001f20: 2020 2020 2073 656c 662e 6c6f 6767 6572       self.logger
-00001f30: 2e65 7272 6f72 2822 5375 6220 4578 6365  .error("Sub Exce
-00001f40: 7074 696f 6e3a 207b 7d22 2e66 6f72 6d61  ption: {}".forma
-00001f50: 7428 6529 290d 0a20 2020 2020 2020 2020  t(e))..         
-00001f60: 2020 2023 2077 6169 7420 6265 666f 7265     # wait before
-00001f70: 2074 7279 2074 6f20 7265 7375 6273 6372   try to resubscr
-00001f80: 6962 650d 0a20 2020 2020 2020 2020 2020  ibe..           
-00001f90: 2069 6620 7365 6c66 2e65 7272 6f72 203d   if self.error =
-00001fa0: 3d20 5472 7565 3a0d 0a20 2020 2020 2020  = True:..       
-00001fb0: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
-00001fc0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00001fd0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001fe0: 2020 2061 7761 6974 2061 7379 6e63 696f     await asyncio
-00001ff0: 2e73 6c65 6570 2835 290d 0a              .sleep(5)..
+00000b20: 2020 2020 2020 2020 6d65 7468 6f64 203d          method =
+00000b30: 2074 6f70 6963 5f66 696c 7465 725b 315d   topic_filter[1]
+00000b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 2020 6966 206d 6573 7361 6765 2e74 6f70    if message.top
+00000b70: 6963 2e6d 6174 6368 6573 2874 6f70 6963  ic.matches(topic
+00000b80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ba0: 2020 2020 2020 2020 6177 6169 7420 286d          await (m
+00000bb0: 6574 686f 6428 6d65 7373 6167 6529 290d  ethod(message)).
+00000bc0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00000bd0: 6570 7420 6173 796e 6369 6f2e 4361 6e63  ept asyncio.Canc
+00000be0: 656c 6c65 6445 7272 6f72 3a0d 0a20 2020  elledError:..   
+00000bf0: 2020 2020 2020 2020 2020 2020 2023 2043               # C
+00000c00: 616e 6365 6c0d 0a20 2020 2020 2020 2020  ancel..         
+00000c10: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
+00000c20: 6572 2e77 6172 6e69 6e67 2822 4d51 5454  er.warning("MQTT
+00000c30: 204c 6973 7465 6e69 6e67 2043 616e 6365   Listening Cance
+00000c40: 6c6c 6564 2229 0d0a 2020 2020 2020 2020  lled")..        
+00000c50: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
+00000c60: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00000c70: 7420 4d71 7474 4572 726f 7220 6173 2065  t MqttError as e
+00000c80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000c90: 2020 2073 656c 662e 6c6f 6767 6572 2e65     self.logger.e
+00000ca0: 7272 6f72 2822 4d51 5454 2045 7863 6570  rror("MQTT Excep
+00000cb0: 7469 6f6e 3a20 7b7d 222e 666f 726d 6174  tion: {}".format
+00000cc0: 2865 2929 0d0a 2020 2020 2020 2020 2020  (e))..          
+00000cd0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00000ce0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
+00000cf0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00000d00: 6f67 6765 722e 6572 726f 7228 224d 5154  ogger.error("MQT
+00000d10: 5420 4765 6e65 7261 6c20 4578 6365 7074  T General Except
+00000d20: 696f 6e3a 207b 7d22 2e66 6f72 6d61 7428  ion: {}".format(
+00000d30: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+00000d40: 2061 7761 6974 2061 7379 6e63 696f 2e73   await asyncio.s
+00000d50: 6c65 6570 2835 290d 0a0d 0a0d 0a20 2020  leep(5)......   
+00000d60: 2061 7379 6e63 2064 6566 2070 7562 6c69   async def publi
+00000d70: 7368 2873 656c 662c 2074 6f70 6963 2c20  sh(self, topic, 
+00000d80: 6d65 7373 6167 652c 2072 6574 6169 6e3d  message, retain=
+00000d90: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00000da0: 2069 6620 7365 6c66 2e63 6c69 656e 7420   if self.client 
+00000db0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00000dc0: 7365 6c66 2e63 6c69 656e 742e 5f63 6f6e  self.client._con
+00000dd0: 6e65 6374 6564 3a0d 0a20 2020 2020 2020  nected:..       
+00000de0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00000df0: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00000e00: 2073 656c 662e 636c 6965 6e74 2e70 7562   self.client.pub
+00000e10: 6c69 7368 2874 6f70 6963 2c20 6d65 7373  lish(topic, mess
+00000e20: 6167 652c 2071 6f73 3d31 2c20 7265 7461  age, qos=1, reta
+00000e30: 696e 3d72 6574 6169 6e29 0d0a 2020 2020  in=retain)..    
+00000e40: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00000e50: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e70: 7365 6c66 2e6c 6f67 6765 722e 7761 726e  self.logger.warn
+00000e80: 696e 6728 2246 6169 6c65 6420 746f 2070  ing("Failed to p
+00000e90: 7573 6820 6461 7461 2076 6961 206d 7174  ush data via mqt
+00000ea0: 743a 207b 7d22 2e66 6f72 6d61 7428 6529  t: {}".format(e)
+00000eb0: 290d 0a0d 0a20 2020 2061 7379 6e63 2064  )....    async d
+00000ec0: 6566 205f 6163 746f 725f 6f6e 2873 656c  ef _actor_on(sel
+00000ed0: 662c 206d 6573 7361 6765 293a 0d0a 2020  f, message):..  
+00000ee0: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f00: 746f 7069 635f 6b65 7920 3d20 7374 7228  topic_key = str(
+00000f10: 6d65 7373 6167 652e 746f 7069 6329 2e73  message.topic).s
+00000f20: 706c 6974 2822 2f22 290d 0a20 2020 2020  plit("/")..     
+00000f30: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00000f40: 2073 656c 662e 6362 7069 2e61 6374 6f72   self.cbpi.actor
+00000f50: 2e6f 6e28 746f 7069 635f 6b65 795b 325d  .on(topic_key[2]
+00000f60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00000f70: 2020 2073 656c 662e 6c6f 6767 6572 2e77     self.logger.w
+00000f80: 6172 6e69 6e67 2822 5072 6f63 6573 7365  arning("Processe
+00000f90: 6420 6163 746f 7220 7b7d 206f 6e20 7669  d actor {} on vi
+00000fa0: 6120 6d71 7474 222e 666f 726d 6174 2874  a mqtt".format(t
+00000fb0: 6f70 6963 5f6b 6579 5b32 5d29 290d 0a20  opic_key[2])).. 
+00000fc0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00000fd0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00000fe0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000ff0: 2020 2073 656c 662e 6c6f 6767 6572 2e77     self.logger.w
+00001000: 6172 6e69 6e67 2822 4661 696c 6564 2074  arning("Failed t
+00001010: 6f20 7072 6f63 6573 7320 6163 746f 7220  o process actor 
+00001020: 6f6e 2076 6961 206d 7174 743a 207b 7d22  on via mqtt: {}"
+00001030: 2e66 6f72 6d61 7428 6529 290d 0a0d 0a20  .format(e)).... 
+00001040: 2020 2061 7379 6e63 2064 6566 205f 6163     async def _ac
+00001050: 746f 725f 6f66 6628 7365 6c66 2c20 6d65  tor_off(self, me
+00001060: 7373 6167 6529 3a0d 0a20 2020 2020 2020  ssage):..       
+00001070: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00001080: 2020 2020 2020 2020 2020 2074 6f70 6963             topic
+00001090: 5f6b 6579 203d 2073 7472 286d 6573 7361  _key = str(messa
+000010a0: 6765 2e74 6f70 6963 292e 7370 6c69 7428  ge.topic).split(
+000010b0: 222f 2229 0d0a 2020 2020 2020 2020 2020  "/")..          
+000010c0: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+000010d0: 2e63 6270 692e 6163 746f 722e 6f66 6628  .cbpi.actor.off(
+000010e0: 746f 7069 635f 6b65 795b 325d 290d 0a20  topic_key[2]).. 
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001100: 656c 662e 6c6f 6767 6572 2e77 6172 6e69  elf.logger.warni
+00001110: 6e67 2822 5072 6f63 6573 7365 6420 6163  ng("Processed ac
+00001120: 746f 7220 7b7d 206f 6666 2076 6961 206d  tor {} off via m
+00001130: 7174 7422 2e66 6f72 6d61 7428 746f 7069  qtt".format(topi
+00001140: 635f 6b65 795b 325d 2929 0d0a 2020 2020  c_key[2]))..    
+00001150: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00001160: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 7365 6c66 2e6c 6f67 6765 722e 7761 726e  self.logger.warn
+00001190: 696e 6728 2246 6169 6c65 6420 746f 2070  ing("Failed to p
+000011a0: 726f 6365 7373 2061 6374 6f72 206f 6666  rocess actor off
+000011b0: 2076 6961 206d 7174 743a 207b 7d22 2e66   via mqtt: {}".f
+000011c0: 6f72 6d61 7428 6529 290d 0a0d 0a20 2020  ormat(e))....   
+000011d0: 2061 7379 6e63 2064 6566 205f 6163 746f   async def _acto
+000011e0: 725f 706f 7765 7228 7365 6c66 2c20 6d65  r_power(self, me
+000011f0: 7373 6167 6529 3a0d 0a20 2020 2020 2020  ssage):..       
+00001200: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00001210: 2020 2020 2020 2020 2020 2074 6f70 6963             topic
+00001220: 5f6b 6579 203d 2073 7472 286d 6573 7361  _key = str(messa
+00001230: 6765 2e74 6f70 6963 292e 7370 6c69 7428  ge.topic).split(
+00001240: 222f 2229 0d0a 2020 2020 2020 2020 2020  "/")..          
+00001250: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
+00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001270: 706f 7765 723d 696e 7428 6d65 7373 6167  power=int(messag
+00001280: 652e 7061 796c 6f61 642e 6465 636f 6465  e.payload.decode
+00001290: 2829 290d 0a20 2020 2020 2020 2020 2020  ())..           
+000012a0: 2020 2020 2020 2020 2069 6620 706f 7765           if powe
+000012b0: 7220 3e20 3130 303a 200d 0a20 2020 2020  r > 100: ..     
+000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012d0: 2020 2070 6f77 6572 203d 2031 3030 0d0a     power = 100..
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 2020 6966 2070 6f77 6572 203c 2030      if power < 0
+00001300: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001310: 2020 2020 2020 2020 2020 2070 6f77 6572             power
+00001320: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
+00001330: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00001340: 7365 6c66 2e63 6270 692e 6163 746f 722e  self.cbpi.actor.
+00001350: 7365 745f 706f 7765 7228 746f 7069 635f  set_power(topic_
+00001360: 6b65 795b 325d 2c70 6f77 6572 290d 0a20  key[2],power).. 
+00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001380: 2020 2023 6177 6169 7420 7365 6c66 2e63     #await self.c
+00001390: 6270 692e 6163 746f 722e 6163 746f 725f  bpi.actor.actor_
+000013a0: 7570 6461 7465 2874 6f70 6963 5f6b 6579  update(topic_key
+000013b0: 5b32 5d2c 706f 7765 7229 0d0a 2020 2020  [2],power)..    
+000013c0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+000013d0: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
+000013e0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+000013f0: 6767 6572 2e77 6172 6e69 6e67 2822 4661  gger.warning("Fa
+00001400: 696c 6564 2074 6f20 7365 7420 6163 746f  iled to set acto
+00001410: 7220 706f 7765 7220 7669 6120 6d71 7474  r power via mqtt
+00001420: 2e20 4e6f 2076 616c 6964 2070 6f77 6572  . No valid power
+00001430: 2069 6e20 6d65 7373 6167 6522 290d 0a20   in message").. 
+00001440: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00001450: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00001460: 2020 2020 7365 6c66 2e6c 6f67 6765 722e      self.logger.
+00001470: 7761 726e 696e 6728 2246 6169 6c65 6420  warning("Failed 
+00001480: 746f 2073 6574 2061 6374 6f72 2070 6f77  to set actor pow
+00001490: 6572 2076 6961 206d 7174 7422 290d 0a0d  er via mqtt")...
+000014a0: 0a20 2020 2061 7379 6e63 2064 6566 205f  .    async def _
+000014b0: 6b65 7474 6c65 7570 6461 7465 2873 656c  kettleupdate(sel
+000014c0: 662c 206d 6573 7361 6765 293a 0d0a 2020  f, message):..  
+000014d0: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014f0: 7365 6c66 2e6b 6574 746c 653d 7365 6c66  self.kettle=self
+00001500: 2e6b 6574 746c 6563 6f6e 7472 6f6c 6c65  .kettlecontrolle
+00001510: 722e 6765 745f 7374 6174 6528 290d 0a20  r.get_state().. 
+00001520: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00001530: 6f72 2069 7465 6d20 696e 2073 656c 662e  or item in self.
+00001540: 6b65 7474 6c65 5b27 6461 7461 275d 3a0d  kettle['data']:.
+00001550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001560: 2020 2020 2073 656c 662e 6362 7069 2e70       self.cbpi.p
+00001570: 7573 685f 7570 6461 7465 2822 6362 7069  ush_update("cbpi
+00001580: 2f7b 7d2f 7b7d 222e 666f 726d 6174 2822  /{}/{}".format("
+00001590: 6b65 7474 6c65 7570 6461 7465 222c 6974  kettleupdate",it
+000015a0: 656d 5b27 6964 275d 292c 2069 7465 6d29  em['id']), item)
+000015b0: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+000015c0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+000015d0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
+000015e0: 2020 2020 2020 7365 6c66 2e6c 6f67 6765        self.logge
+000015f0: 722e 7761 726e 696e 6728 2246 6169 6c65  r.warning("Faile
+00001600: 6420 746f 2073 656e 6420 6b65 7474 6c65  d to send kettle
+00001610: 7570 6461 7465 2076 6961 206d 7174 743a  update via mqtt:
+00001620: 207b 7d22 2e66 6f72 6d61 7428 6529 290d   {}".format(e)).
+00001630: 0a0d 0a20 2020 2061 7379 6e63 2064 6566  ...    async def
+00001640: 205f 6665 726d 656e 7465 7275 7064 6174   _fermenterupdat
+00001650: 6528 7365 6c66 2c20 6d65 7373 6167 6529  e(self, message)
+00001660: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+00001670: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00001680: 2020 2020 2073 656c 662e 6665 726d 656e       self.fermen
+00001690: 7465 723d 7365 6c66 2e66 6572 6d65 6e74  ter=self.ferment
+000016a0: 6572 636f 6e74 726f 6c6c 6572 2e67 6574  ercontroller.get
+000016b0: 5f73 7461 7465 2829 0d0a 2020 2020 2020  _state()..      
+000016c0: 2020 2020 2020 2020 2020 666f 7220 6974            for it
+000016d0: 656d 2069 6e20 7365 6c66 2e66 6572 6d65  em in self.ferme
+000016e0: 6e74 6572 5b27 6461 7461 275d 3a0d 0a20  nter['data']:.. 
+000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001700: 2020 2069 7465 6d5f 6e65 773d 7365 6c66     item_new=self
+00001710: 2e72 656d 6f76 655f 6b65 7928 6974 656d  .remove_key(item
+00001720: 2c22 7374 6570 7322 290d 0a20 2020 2020  ,"steps")..     
+00001730: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001740: 656c 662e 6362 7069 2e70 7573 685f 7570  elf.cbpi.push_up
+00001750: 6461 7465 2822 6362 7069 2f7b 7d2f 7b7d  date("cbpi/{}/{}
+00001760: 222e 666f 726d 6174 2822 6665 726d 656e  ".format("fermen
+00001770: 7465 7275 7064 6174 6522 2c69 7465 6d5b  terupdate",item[
+00001780: 2769 6427 5d29 2c20 6974 656d 5f6e 6577  'id']), item_new
+00001790: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+000017a0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+000017b0: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
+000017c0: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
+000017d0: 6572 2e77 6172 6e69 6e67 2822 4661 696c  er.warning("Fail
+000017e0: 6564 2074 6f20 7365 6e64 2066 6572 6d65  ed to send ferme
+000017f0: 6e74 6572 7570 6461 7465 2076 6961 206d  nterupdate via m
+00001800: 7174 743a 207b 7d22 2e66 6f72 6d61 7428  qtt: {}".format(
+00001810: 6529 290d 0a0d 0a20 2020 2061 7379 6e63  e))....    async
+00001820: 2064 6566 205f 6163 746f 7275 7064 6174   def _actorupdat
+00001830: 6528 7365 6c66 2c20 6d65 7373 6167 6529  e(self, message)
+00001840: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+00001850: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00001860: 2020 2020 2073 656c 662e 6163 746f 723d       self.actor=
+00001870: 7365 6c66 2e61 6374 6f72 636f 6e74 726f  self.actorcontro
+00001880: 6c6c 6572 2e67 6574 5f73 7461 7465 2829  ller.get_state()
+00001890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000018a0: 2020 666f 7220 6974 656d 2069 6e20 7365    for item in se
+000018b0: 6c66 2e61 6374 6f72 5b27 6461 7461 275d  lf.actor['data']
+000018c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000018d0: 2020 2020 2020 2073 656c 662e 6362 7069         self.cbpi
+000018e0: 2e70 7573 685f 7570 6461 7465 2822 6362  .push_update("cb
+000018f0: 7069 2f7b 7d2f 7b7d 222e 666f 726d 6174  pi/{}/{}".format
+00001900: 2822 6163 746f 7275 7064 6174 6522 2c69  ("actorupdate",i
+00001910: 7465 6d5b 2769 6427 5d29 2c20 6974 656d  tem['id']), item
+00001920: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00001930: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00001940: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
+00001950: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
+00001960: 6572 2e77 6172 6e69 6e67 2822 4661 696c  er.warning("Fail
+00001970: 6564 2074 6f20 7365 6e64 2061 6374 6f72  ed to send actor
+00001980: 7570 6461 7465 2076 6961 206d 7174 743a  update via mqtt:
+00001990: 207b 7d22 2e66 6f72 6d61 7428 6529 290d   {}".format(e)).
+000019a0: 0a0d 0a20 2020 2061 7379 6e63 2064 6566  ...    async def
+000019b0: 205f 7365 6e73 6f72 7570 6461 7465 2873   _sensorupdate(s
+000019c0: 656c 662c 206d 6573 7361 6765 293a 0d0a  elf, message):..
+000019d0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+000019e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000019f0: 2020 7365 6c66 2e73 656e 736f 723d 7365    self.sensor=se
+00001a00: 6c66 2e73 656e 736f 7263 6f6e 7472 6f6c  lf.sensorcontrol
+00001a10: 6c65 722e 6765 745f 7374 6174 6528 290d  ler.get_state().
+00001a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a30: 2066 6f72 2069 7465 6d20 696e 2073 656c   for item in sel
+00001a40: 662e 7365 6e73 6f72 5b27 6461 7461 275d  f.sensor['data']
+00001a50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001a60: 2020 2020 2020 2073 656c 662e 6362 7069         self.cbpi
+00001a70: 2e70 7573 685f 7570 6461 7465 2822 6362  .push_update("cb
+00001a80: 7069 2f7b 7d2f 7b7d 222e 666f 726d 6174  pi/{}/{}".format
+00001a90: 2822 7365 6e73 6f72 7570 6461 7465 222c  ("sensorupdate",
+00001aa0: 6974 656d 5b27 6964 275d 292c 2069 7465  item['id']), ite
+00001ab0: 6d29 0d0a 2020 2020 2020 2020 2020 2020  m)..            
+00001ac0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00001ad0: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+00001ae0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+00001af0: 6765 722e 7761 726e 696e 6728 2246 6169  ger.warning("Fai
+00001b00: 6c65 6420 746f 2073 656e 6420 7365 6e73  led to send sens
+00001b10: 6f72 7570 6461 7465 2076 6961 206d 7174  orupdate via mqt
+00001b20: 743a 207b 7d22 2e66 6f72 6d61 7428 6529  t: {}".format(e)
+00001b30: 290d 0a0d 0a20 2020 2064 6566 2073 7562  )....    def sub
+00001b40: 7363 7269 6265 2873 656c 662c 2074 6f70  scribe(self, top
+00001b50: 6963 2c20 6d65 7468 6f64 293a 0d0a 2020  ic, method):..  
+00001b60: 2020 2020 2020 7365 6c66 2e74 6f70 6963        self.topic
+00001b70: 5f66 696c 7465 7273 2e61 7070 656e 6428  _filters.append(
+00001b80: 2874 6f70 6963 2c6d 6574 686f 6429 290d  (topic,method)).
+00001b90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001ba0: 5472 7565 0d0a 2020 2020 0d0a 2020 2020  True..    ..    
+00001bb0: 6465 6620 756e 7375 6273 6372 6962 6528  def unsubscribe(
+00001bc0: 7365 6c66 2c20 746f 7069 632c 206d 6574  self, topic, met
+00001bd0: 686f 6429 3a0d 0a20 2020 2020 2020 2073  hod):..        s
+00001be0: 656c 662e 746f 7069 635f 6669 6c74 6572  elf.topic_filter
+00001bf0: 732e 7265 6d6f 7665 2828 746f 7069 632c  s.remove((topic,
+00001c00: 6d65 7468 6f64 2929 0d0a 2020 2020 2020  method))..      
+00001c10: 2020 7265 7475 726e 2054 7275 650d 0a      return True..
```

### Comparing `cbpi4-4.3.2/cbpi/controller/sensor_controller.py` & `cbpi4-4.4.0/cbpi/controller/sensor_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/step_controller.py` & `cbpi4-4.4.0/cbpi/controller/step_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/system_controller.py` & `cbpi4-4.4.0/cbpi/controller/system_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/controller/upload_controller.py` & `cbpi4-4.4.0/cbpi/controller/upload_controller.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/craftbeerpi.py` & `cbpi4-4.4.0/cbpi/craftbeerpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
             await i["method"]()
 
     def _print_logo(self):
         from pyfiglet import Figlet
         f = Figlet(font='big')
         logger.warning("\n%s" % f.renderText("CraftBeerPi %s " % self.version))
         logger.warning("www.CraftBeerPi.com")
-        logger.warning("(c) 2021/2022/2023 Manuel Fritsch / Alexander Vollkopf")
+        logger.warning("(c) 2021 - 2024 Manuel Fritsch / Alexander Vollkopf")
 
     def _setup_http_index(self):
         async def http_index(request):
             url = self.config.static.get("index_url")
 
             if url is not None:
```

### Comparing `cbpi4-4.3.2/cbpi/eventbus.py` & `cbpi4-4.4.0/cbpi/eventbus.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__init__.py` & `cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/ConfigUpdate/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermentationStep/__init__.py` & `cbpi4-4.4.0/cbpi/extension/FermentationStep/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/FermentationStep/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__init__.py` & `cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/FermenterHysteresis/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/SensorLogTarget_CSV/__init__.py` & `cbpi4-4.4.0/cbpi/extension/SensorLogTarget_CSV/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/SensorLogTarget_CSV/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/SensorLogTarget_CSV/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/SensorLogTarget_CSV/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/SensorLogTarget_CSV/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/SensorLogTarget_InfluxDB/__init__.py` & `cbpi4-4.4.0/cbpi/extension/SensorLogTarget_InfluxDB/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/SensorLogTarget_InfluxDB/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummyactor/__init__.py` & `cbpi4-4.4.0/cbpi/extension/dummyactor/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummyactor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/dummyactor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummyactor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/dummyactor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummyactor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/dummyactor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummyactor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/dummyactor/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummysensor/__init__.py` & `cbpi4-4.4.0/cbpi/extension/dummysensor/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummysensor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/dummysensor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummysensor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/dummysensor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummysensor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/dummysensor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/dummysensor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/dummysensor/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/gpioactor/__init__.py` & `cbpi4-4.4.0/cbpi/extension/gpioactor/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -93,15 +93,17 @@
 
     async def set_power(self, power):
         self.power = power
         await self.cbpi.actor.actor_update(self.id,power)
         pass
             
 
-@parameters([Property.Select(label="GPIO", options=[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27]), Property.Number(label="Frequency", configurable=True)])
+@parameters([Property.Select(label="GPIO", options=[0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27]), 
+             Property.Number(label="Frequency", configurable=True),
+             Property.Select(label="Inverted",options=["Yes","No"],description="Inverts PWM load if set to yes (e.g. 90% = 10%). Default: No")])
 class GPIOPWMActor(CBPiActor):
 
     # Custom property which can be configured by the user
     @action("Set Power", parameters=[Property.Number(label="Power", configurable=True,description="Power Setting [0-100]")])
     async def setpower(self,Power = 100 ,**kwargs):
         logging.info(Power)
         self.power=int(Power)
@@ -109,18 +111,22 @@
             self.power = 0
         if self.power > 100:
             self.power = 100           
         await self.set_power(self.power)
 
     async def on_start(self):
         self.gpio = self.props.get("GPIO", None)
+        self.inverted = self.props.get("Inverted", "No")
         self.frequency = self.props.get("Frequency", 0.5)
         if self.gpio is not None:
             GPIO.setup(self.gpio, GPIO.OUT)
-            GPIO.output(self.gpio, 0)
+            if self.inverted == "No":
+                GPIO.output(self.gpio, 0)
+            else:
+                GPIO.output(self.gpio, 1)
         self.state = False
         self.power = None
         self.p = None
         pass
 
     async def on(self, power = None):
         logging.debug("PWM Actor Power: {}".format(power))
@@ -131,28 +137,38 @@
 
         logging.debug("PWM Final Power: {}".format(self.power))    
         
         logger.debug("PWM ACTOR %s ON - GPIO %s - Frequency %s - Power %s" %  (self.id, self.gpio,self.frequency,self.power))
         try:
             if self.p is None:
                 self.p = GPIO.PWM(int(self.gpio), float(self.frequency))
-            self.p.start(self.power)
+            if self.inverted == "No":
+                self.p.start(self.power)
+            else:
+                self.p.start(100- self.power)
             self.state = True
 #            await self.cbpi.actor.actor_update(self.id,self.power)
         except:
             pass
 
     async def off(self):
         logger.info("PWM ACTOR %s OFF - GPIO %s " % (self.id, self.gpio))
-        self.p.ChangeDutyCycle(0)
+        if self.inverted == "No":
+            self.p.ChangeDutyCycle(0)
+        else:
+            self.p.ChangeDutyCycle(100)
+
         self.state = False
 
     async def set_power(self, power):
         if self.p and self.state == True:
-            self.p.ChangeDutyCycle(power)
+            if self.inverted == "No":          
+                self.p.ChangeDutyCycle(power)
+            else:
+                self.p.ChangeDutyCycle(100 - power) # Set power to 100-value to invert output
         await self.cbpi.actor.actor_update(self.id,power)
         pass
 
     def get_state(self):
         return self.state
     
     async def run(self):
```

### Comparing `cbpi4-4.3.2/cbpi/extension/gpioactor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/gpioactor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/gpioactor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/gpioactor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/gpioactor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/gpioactor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/gpioactor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/gpioactor/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Mar 10 17:08:18 2023 UTC, .py size: 6111 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 0264 0b64 df17 0000  a........d.d....
+00000000: 610d 0d0a 0000 0000 be0f de65 971a 0000  a..........e....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 3a01 0000 6400  .....@...s:...d.
+00000020: 0008 0000 0040 0000 0073 4c01 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 5400 6501 a006 6507 a101 5a08  d.l.T.e...e...Z.
 00000060: 7a10 6400 6401 6c09 6d0a 5a0a 0100 5700  z.d.d.l.m.Z...W.
 00000070: 6e4e 0400 650b 7990 0100 0100 0100 6508  nN..e.y.......e.
 00000080: a00c 6404 a101 0100 6503 8300 5a0d 650d  ..d.....e...Z.e.
 00000090: 650d 6a0a 6405 9c02 5a0e 6504 a00f 6406  e.j.d...Z.e...d.
@@ -14,346 +14,364 @@
 000000d0: 650a a014 650a 6a15 a101 0100 6516 6517  e...e.j.....e.e.
 000000e0: 6a18 6407 6700 6408 a201 6409 8d02 6517  j.d.g.d...d...e.
 000000f0: 6a18 640a 640b 640c 6702 640d 640e 8d03  j.d.d.d.g.d.d...
 00000100: 6517 6a18 640f 6410 6411 6702 6412 640e  e.j.d.d.d.g.d.d.
 00000110: 8d03 6703 8301 4700 6413 6414 8400 6414  ..g...G.d.d...d.
 00000120: 6519 8303 8301 5a1a 6516 6517 6a18 6407  e.....Z.e.e.j.d.
 00000130: 6700 6408 a201 6409 8d02 6517 6a1b 6415  g.d...d...e.j.d.
-00000140: 6416 6417 8d02 6702 8301 4700 6418 6419  d.d...g...G.d.d.
-00000150: 8400 6419 6519 8303 8301 5a1c 641a 641b  ..d.e.....Z.d.d.
-00000160: 8400 5a1d 6401 5300 291c e900 0000 004e  ..Z.d.S.)......N
-00000170: 2902 da09 4d61 6769 634d 6f63 6bda 0570  )...MagicMock..p
-00000180: 6174 6368 2901 da01 2a7a 2b46 6169 6c65  atch)...*z+Faile
-00000190: 6420 746f 206c 6f61 6420 5250 692e 4750  d to load RPi.GP
-000001a0: 494f 2e20 5573 696e 6720 4d6f 636b 2069  IO. Using Mock i
-000001b0: 6e73 7465 6164 2902 5a03 5250 697a 0852  nstead).Z.RPiz.R
-000001c0: 5069 2e47 5049 4f7a 0b73 7973 2e6d 6f64  Pi.GPIOz.sys.mod
-000001d0: 756c 6573 da04 4750 494f 291c 7201 0000  ules..GPIO).r...
-000001e0: 00e9 0100 0000 e902 0000 00e9 0300 0000  ................
-000001f0: e904 0000 00e9 0500 0000 e906 0000 00e9  ................
-00000200: 0700 0000 e908 0000 00e9 0900 0000 e90a  ................
-00000210: 0000 00e9 0b00 0000 e90c 0000 00e9 0d00  ................
-00000220: 0000 e90e 0000 00e9 0f00 0000 e910 0000  ................
-00000230: 00e9 1100 0000 e912 0000 00e9 1300 0000  ................
-00000240: e914 0000 00e9 1500 0000 e916 0000 00e9  ................
-00000250: 1700 0000 e918 0000 00e9 1900 0000 e91a  ................
-00000260: 0000 00e9 1b00 0000 2902 da05 6c61 6265  ........)...labe
-00000270: 6cda 076f 7074 696f 6e73 da08 496e 7665  l..options..Inve
-00000280: 7274 6564 da03 5965 73da 024e 6f7a 264e  rted..Yes..Noz&N
-00000290: 6f3a 2041 6374 6976 6520 6f6e 2068 6967  o: Active on hig
-000002a0: 683b 2059 6573 3a20 4163 7469 7665 206f  h; Yes: Active o
-000002b0: 6e20 6c6f 7729 0372 2100 0000 7222 0000  n low).r!...r"..
-000002c0: 00da 0b64 6573 6372 6970 7469 6f6e da0c  ...description..
-000002d0: 5361 6d70 6c69 6e67 5469 6d65 7207 0000  SamplingTimer...
-000002e0: 0072 0a00 0000 7a33 5469 6d65 2069 6e20  .r....z3Time in 
-000002f0: 7365 636f 6e64 7320 666f 7220 706f 7765  seconds for powe
-00000300: 7220 6261 7365 2069 6e74 6572 7661 6c20  r base interval 
-00000310: 2844 6566 6175 6c74 3a35 2963 0000 0000  (Default:5)c....
-00000320: 0000 0000 0000 0000 0000 0000 0700 0000  ................
-00000330: 4000 0000 736a 0000 0065 005a 0164 005a  @...sj...e.Z.d.Z
-00000340: 0265 0364 0165 046a 0564 0264 0364 0464  .e.d.e.j.d.d.d.d
-00000350: 058d 0367 0164 068d 0264 1964 0864 0984  ...g.d...d.d.d..
-00000360: 0183 015a 0664 0a64 0b84 005a 0764 0c64  ...Z.d.d...Z.d.d
-00000370: 0d84 005a 0864 1a64 0f64 1084 015a 0964  ...Z.d.d.d...Z.d
-00000380: 1164 1284 005a 0a64 1364 1484 005a 0b64  .d...Z.d.d...Z.d
-00000390: 1564 1684 005a 0c64 1764 1884 005a 0d64  .d...Z.d.d...Z.d
-000003a0: 0e53 0029 1bda 0947 5049 4f41 6374 6f72  .S.)...GPIOActor
-000003b0: fa09 5365 7420 506f 7765 72da 0550 6f77  ..Set Power..Pow
-000003c0: 6572 54fa 1550 6f77 6572 2053 6574 7469  erT..Power Setti
-000003d0: 6e67 205b 302d 3130 305d a903 7221 0000  ng [0-100]..r!..
-000003e0: 00da 0c63 6f6e 6669 6775 7261 626c 6572  ...configurabler
-000003f0: 2600 0000 a901 da0a 7061 7261 6d65 7465  &.......paramete
-00000400: 7273 e964 0000 0063 0200 0000 0000 0000  rs.d...c........
-00000410: 0000 0000 0300 0000 0300 0000 cb00 0000  ................
-00000420: 7340 0000 0074 007c 0183 017c 005f 017c  s@...t.|...|._.|
-00000430: 006a 0164 016b 0072 1a64 017c 005f 017c  .j.d.k.r.d.|._.|
-00000440: 006a 0164 026b 0472 2a64 027c 005f 017c  .j.d.k.r*d.|._.|
-00000450: 00a0 027c 006a 01a1 0149 0064 0048 0001  ...|.j...I.d.H..
-00000460: 0064 0053 00a9 034e 7201 0000 0072 3000  .d.S...Nr....r0.
-00000470: 0000 2903 da03 696e 74da 0570 6f77 6572  ..)...int..power
-00000480: da09 7365 745f 706f 7765 72a9 03da 0473  ..set_power....s
-00000490: 656c 6672 2a00 0000 da06 6b77 6172 6773  elfr*.....kwargs
-000004a0: a900 7238 0000 00fa 5863 3a5c 7573 6572  ..r8....Xc:\user
-000004b0: 735c 616c 6578 616e 6465 725c 646f 776e  s\alexander\down
-000004c0: 6c6f 6164 735c 6372 6166 7462 6565 7270  loads\craftbeerp
-000004d0: 6934 5f61 766f 6c6c 6b6f 7066 5c63 6270  i4_avollkopf\cbp
-000004e0: 695c 6578 7465 6e73 696f 6e5c 6770 696f  i\extension\gpio
-000004f0: 6163 746f 725c 5f5f 696e 6974 5f5f 2e70  actor\__init__.p
-00000500: 79da 0873 6574 706f 7765 7221 0000 0073  y..setpower!...s
-00000510: 0c00 0000 0002 0a01 0a01 0601 0a01 0601  ................
-00000520: 7a12 4750 494f 4163 746f 722e 7365 7470  z.GPIOActor.setp
-00000530: 6f77 6572 6302 0000 0000 0000 0000 0000  owerc...........
-00000540: 0002 0000 0002 0000 0043 0000 0073 3800  .........C...s8.
-00000550: 0000 7c01 6401 6b02 721a 7c00 6a00 6402  ..|.d.k.r.|.j.d.
-00000560: 6b02 7216 6401 5300 6403 5300 7c01 6403  k.r.d.S.d.S.|.d.
-00000570: 6b02 7234 7c00 6a00 6402 6b02 7230 6403  k.r4|.j.d.k.r0d.
-00000580: 5300 6401 5300 6400 5300 2904 4e72 0600  S.d.S.d.S.).Nr..
-00000590: 0000 4672 0100 0000 2901 da08 696e 7665  ..Fr....)...inve
-000005a0: 7274 6564 2902 7236 0000 00da 0573 7461  rted).r6.....sta
-000005b0: 7465 7238 0000 0072 3800 0000 7239 0000  ter8...r8...r9..
-000005c0: 00da 0e67 6574 5f47 5049 4f5f 7374 6174  ...get_GPIO_stat
-000005d0: 652a 0000 0073 0800 0000 0002 0801 1202  e*...s..........
-000005e0: 0801 7a18 4750 494f 4163 746f 722e 6765  ..z.GPIOActor.ge
-000005f0: 745f 4750 494f 5f73 7461 7465 6301 0000  t_GPIO_statec...
-00000600: 0000 0000 0000 0000 0001 0000 0006 0000  ................
-00000610: 00c3 0000 0073 6e00 0000 6400 7c00 5f00  .....sn...d.|._.
-00000620: 7c00 6a01 6a02 7c00 5f03 7c00 6a01 a004  |.j.j.|._.|.j...
-00000630: 6401 6402 a102 6403 6b02 7226 6404 6e02  d.d...d.k.r&d.n.
-00000640: 6405 7c00 5f05 7406 7c00 6a01 a004 6406  d.|._.t.|.j...d.
-00000650: 6407 a102 8301 7c00 5f07 7402 a008 7c00  d.....|._.t...|.
-00000660: 6a03 7402 6a09 a102 0100 7402 a00a 7c00  j.t.j.....t...|.
-00000670: 6a03 7c00 a00b 6408 a101 a102 0100 6405  j.|...d.......d.
-00000680: 7c00 5f0c 6400 5300 2909 4e72 2300 0000  |._.d.S.).Nr#...
-00000690: 7225 0000 0072 2400 0000 5446 7227 0000  r%...r$...TFr'..
-000006a0: 0072 0a00 0000 7201 0000 0029 0d72 3300  .r....r....).r3.
-000006b0: 0000 da05 7072 6f70 7372 0500 0000 da04  ....propsr......
-000006c0: 6770 696f da03 6765 7472 3b00 0000 7232  gpio..getr;...r2
-000006d0: 0000 00da 0a73 616d 706c 6554 696d 65da  .....sampleTime.
-000006e0: 0573 6574 7570 da03 4f55 54da 066f 7574  .setup..OUT..out
-000006f0: 7075 7472 3d00 0000 723c 0000 00a9 0172  putr=...r<.....r
-00000700: 3600 0000 7238 0000 0072 3800 0000 7239  6...r8...r8...r9
-00000710: 0000 00da 086f 6e5f 7374 6172 7432 0000  .....on_start2..
-00000720: 0073 0e00 0000 0001 0601 0a01 1c01 1401  .s..............
-00000730: 1001 1401 7a12 4750 494f 4163 746f 722e  ....z.GPIOActor.
-00000740: 6f6e 5f73 7461 7274 4e63 0200 0000 0000  on_startNc......
-00000750: 0000 0000 0000 0200 0000 0600 0000 c300  ................
-00000760: 0000 734a 0000 007c 0164 0075 0172 107c  ..sJ...|.d.u.r.|
-00000770: 017c 005f 006e 0664 017c 005f 0074 01a0  .|._.n.d.|._.t..
-00000780: 0264 027c 006a 037c 006a 0466 0216 00a1  .d.|.j.|.j.f....
-00000790: 0101 0074 05a0 067c 006a 047c 00a0 0764  ...t...|.j.|...d
-000007a0: 03a1 01a1 0201 0064 047c 005f 0864 0053  .......d.|._.d.S
-000007b0: 0029 054e 7230 0000 007a 1641 4354 4f52  .).Nr0...z.ACTOR
-000007c0: 2025 7320 4f4e 202d 2047 5049 4f20 2573   %s ON - GPIO %s
-000007d0: 2072 0600 0000 5429 0972 3300 0000 da06   r....T).r3.....
-000007e0: 6c6f 6767 6572 da04 696e 666f da02 6964  logger..info..id
-000007f0: 723f 0000 0072 0500 0000 7244 0000 0072  r?...r....rD...r
-00000800: 3d00 0000 723c 0000 00a9 0272 3600 0000  =...r<.....r6...
-00000810: 7233 0000 0072 3800 0000 7238 0000 0072  r3...r8...r8...r
-00000820: 3900 0000 da02 6f6e 3b00 0000 730c 0000  9.....on;...s...
-00000830: 0000 0108 0108 0206 0316 0114 017a 0c47  .............z.G
-00000840: 5049 4f41 6374 6f72 2e6f 6e63 0100 0000  PIOActor.onc....
-00000850: 0000 0000 0000 0000 0100 0000 0600 0000  ................
-00000860: c300 0000 7334 0000 0074 00a0 0164 017c  ....s4...t...d.|
-00000870: 006a 027c 006a 0366 0216 00a1 0101 0074  .j.|.j.f.......t
-00000880: 04a0 057c 006a 037c 00a0 0664 02a1 01a1  ...|.j.|...d....
-00000890: 0201 0064 037c 005f 0764 0053 0029 044e  ...d.|._.d.S.).N
-000008a0: 7a17 4143 544f 5220 2573 204f 4646 202d  z.ACTOR %s OFF -
-000008b0: 2047 5049 4f20 2573 2072 0100 0000 4629   GPIO %s r....F)
-000008c0: 0872 4700 0000 7248 0000 0072 4900 0000  .rG...rH...rI...
-000008d0: 723f 0000 0072 0500 0000 7244 0000 0072  r?...r....rD...r
-000008e0: 3d00 0000 723c 0000 0072 4500 0000 7238  =...r<...rE...r8
-000008f0: 0000 0072 3800 0000 7239 0000 00da 036f  ...r8...r9.....o
-00000900: 6666 4600 0000 7306 0000 0000 0116 0114  ffF...s.........
-00000910: 017a 0d47 5049 4f41 6374 6f72 2e6f 6666  .z.GPIOActor.off
-00000920: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000930: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
-00000940: 6a00 5300 a901 4ea9 0172 3c00 0000 7245  j.S...N..r<...rE
-00000950: 0000 0072 3800 0000 7238 0000 0072 3900  ...r8...r8...r9.
-00000960: 0000 da09 6765 745f 7374 6174 654b 0000  ....get_stateK..
-00000970: 0073 0200 0000 0001 7a13 4750 494f 4163  .s......z.GPIOAc
-00000980: 746f 722e 6765 745f 7374 6174 6563 0100  tor.get_statec..
-00000990: 0000 0000 0000 0000 0000 0300 0000 0600  ................
-000009a0: 0000 c300 0000 739e 0000 007c 006a 0064  ......s....|.j.d
-000009b0: 016b 0272 9a7c 006a 0164 016b 0272 887c  .k.r.|.j.d.k.r.|
-000009c0: 006a 027c 006a 0364 021b 0014 007d 017c  .j.|.j.d.....}.|
-000009d0: 006a 027c 0118 007d 027c 0164 036b 0472  .j.|...}.|.d.k.r
-000009e0: 5a74 04a0 057c 006a 067c 00a0 0764 04a1  Zt...|.j.|...d..
-000009f0: 01a1 0201 0074 08a0 097c 01a1 0149 0064  .....t...|...I.d
-00000a00: 0048 0001 007c 0264 036b 0472 9874 04a0  .H...|.d.k.r.t..
-00000a10: 057c 006a 067c 00a0 0764 03a1 01a1 0201  .|.j.|...d......
-00000a20: 0074 08a0 097c 02a1 0149 0064 0048 0001  .t...|...I.d.H..
-00000a30: 0071 0074 08a0 0964 04a1 0149 0064 0048  .q.t...d...I.d.H
-00000a40: 0001 0071 0064 0053 0029 054e 5472 3000  ...q.d.S.).NTr0.
-00000a50: 0000 7201 0000 0072 0600 0000 290a da07  ..r....r....)...
-00000a60: 7275 6e6e 696e 6772 3c00 0000 7241 0000  runningr<...rA..
-00000a70: 0072 3300 0000 7205 0000 0072 4400 0000  .r3...r....rD...
-00000a80: 723f 0000 0072 3d00 0000 da07 6173 796e  r?...r=.....asyn
-00000a90: 6369 6fda 0573 6c65 6570 2903 7236 0000  cio..sleep).r6..
-00000aa0: 005a 0c68 6561 7469 6e67 5f74 696d 655a  .Z.heating_timeZ
-00000ab0: 0977 6169 745f 7469 6d65 7238 0000 0072  .wait_timer8...r
-00000ac0: 3800 0000 7239 0000 00da 0372 756e 4e00  8...r9.....runN.
-00000ad0: 0000 7316 0000 0000 010a 010a 0110 010a  ..s.............
-00000ae0: 0108 0214 0110 0108 0214 0112 027a 0d47  .............z.G
-00000af0: 5049 4f41 6374 6f72 2e72 756e 6302 0000  PIOActor.runc...
-00000b00: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000b10: 00c3 0000 0073 2200 0000 7c01 7c00 5f00  .....s"...|.|._.
-00000b20: 7c00 6a01 6a02 a003 7c00 6a04 7c01 a102  |.j.j...|.j.|...
-00000b30: 4900 6400 4800 0100 6400 5300 724d 0000  I.d.H...d.S.rM..
-00000b40: 0029 0572 3300 0000 da04 6362 7069 da05  .).r3.....cbpi..
-00000b50: 6163 746f 72da 0c61 6374 6f72 5f75 7064  actor..actor_upd
-00000b60: 6174 6572 4900 0000 724a 0000 0072 3800  aterI...rJ...r8.
-00000b70: 0000 7238 0000 0072 3900 0000 7234 0000  ..r8...r9...r4..
-00000b80: 005e 0000 0073 0600 0000 0001 0601 1801  .^...s..........
-00000b90: 7a13 4750 494f 4163 746f 722e 7365 745f  z.GPIOActor.set_
-00000ba0: 706f 7765 7229 0172 3000 0000 2901 4e29  power).r0...).N)
-00000bb0: 0eda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000bc0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000bd0: 616d 655f 5fda 0661 6374 696f 6eda 0850  ame__..action..P
-00000be0: 726f 7065 7274 79da 064e 756d 6265 7272  roperty..Numberr
-00000bf0: 3a00 0000 723d 0000 0072 4600 0000 724b  :...r=...rF...rK
-00000c00: 0000 0072 4c00 0000 724f 0000 0072 5300  ...rL...rO...rS.
-00000c10: 0000 7234 0000 0072 3800 0000 7238 0000  ..r4...r8...r8..
-00000c20: 0072 3800 0000 7239 0000 0072 2800 0000  .r8...r9...r(...
-00000c30: 1b00 0000 7312 0000 0008 0618 010c 0808  ....s...........
-00000c40: 0808 090a 0b08 0508 0308 1072 2800 0000  ...........r(...
-00000c50: da09 4672 6571 7565 6e63 7954 2902 7221  ..FrequencyT).r!
-00000c60: 0000 0072 2d00 0000 6300 0000 0000 0000  ...r-...c.......
-00000c70: 0000 0000 0000 0000 0007 0000 0040 0000  .............@..
-00000c80: 0073 6200 0000 6500 5a01 6400 5a02 6503  .sb...e.Z.d.Z.e.
-00000c90: 6401 6504 6a05 6402 6403 6404 6405 8d03  d.e.j.d.d.d.d...
-00000ca0: 6701 6406 8d02 6417 6408 6409 8401 8301  g.d...d.d.d.....
-00000cb0: 5a06 640a 640b 8400 5a07 6418 640d 640e  Z.d.d...Z.d.d.d.
-00000cc0: 8401 5a08 640f 6410 8400 5a09 6411 6412  ..Z.d.d...Z.d.d.
-00000cd0: 8400 5a0a 6413 6414 8400 5a0b 6415 6416  ..Z.d.d...Z.d.d.
-00000ce0: 8400 5a0c 640c 5300 2919 da0c 4750 494f  ..Z.d.S.)...GPIO
-00000cf0: 5057 4d41 6374 6f72 7229 0000 0072 2a00  PWMActorr)...r*.
-00000d00: 0000 5472 2b00 0000 722c 0000 0072 2e00  ..Tr+...r,...r..
-00000d10: 0000 7230 0000 0063 0200 0000 0000 0000  ..r0...c........
-00000d20: 0000 0000 0300 0000 0300 0000 cb00 0000  ................
-00000d30: 734a 0000 0074 00a0 017c 01a1 0101 0074  sJ...t...|.....t
-00000d40: 027c 0183 017c 005f 037c 006a 0364 016b  .|...|._.|.j.d.k
-00000d50: 0072 2464 017c 005f 037c 006a 0364 026b  .r$d.|._.|.j.d.k
-00000d60: 0472 3464 027c 005f 037c 00a0 047c 006a  .r4d.|._.|...|.j
-00000d70: 03a1 0149 0064 0048 0001 0064 0053 0072  ...I.d.H...d.S.r
-00000d80: 3100 0000 2905 da07 6c6f 6767 696e 6772  1...)...loggingr
-00000d90: 4800 0000 7232 0000 0072 3300 0000 7234  H...r2...r3...r4
-00000da0: 0000 0072 3500 0000 7238 0000 0072 3800  ...r5...r8...r8.
-00000db0: 0000 7239 0000 0072 3a00 0000 6800 0000  ..r9...r:...h...
-00000dc0: 730e 0000 0000 020a 010a 010a 0106 010a  s...............
-00000dd0: 0106 017a 1547 5049 4f50 574d 4163 746f  ...z.GPIOPWMActo
-00000de0: 722e 7365 7470 6f77 6572 6301 0000 0000  r.setpowerc.....
-00000df0: 0000 0000 0000 0001 0000 0004 0000 00c3  ................
-00000e00: 0000 0073 5e00 0000 7c00 6a00 a001 6401  ...s^...|.j...d.
-00000e10: 6400 a102 7c00 5f02 7c00 6a00 a001 6402  d...|._.|.j...d.
-00000e20: 6403 a102 7c00 5f03 7c00 6a02 6400 7501  d...|._.|.j.d.u.
-00000e30: 7248 7404 a005 7c00 6a02 7404 6a06 a102  rHt...|.j.t.j...
-00000e40: 0100 7404 a007 7c00 6a02 6404 a102 0100  ..t...|.j.d.....
-00000e50: 6405 7c00 5f08 6400 7c00 5f09 6400 7c00  d.|._.d.|._.d.|.
-00000e60: 5f0a 6400 5300 2906 4e72 0500 0000 725d  _.d.S.).Nr....r]
-00000e70: 0000 0067 0000 0000 0000 e03f 7201 0000  ...g.......?r...
-00000e80: 0046 290b 723e 0000 0072 4000 0000 723f  .F).r>...r@...r?
-00000e90: 0000 00da 0966 7265 7175 656e 6379 7205  .....frequencyr.
-00000ea0: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
-00000eb0: 0000 723c 0000 0072 3300 0000 da01 7072  ..r<...r3.....pr
-00000ec0: 4500 0000 7238 0000 0072 3800 0000 7239  E...r8...r8...r9
-00000ed0: 0000 0072 4600 0000 7200 0000 7312 0000  ...rF...r...s...
-00000ee0: 0000 0110 0110 010a 0110 010e 0106 0106  ................
-00000ef0: 0106 017a 1547 5049 4f50 574d 4163 746f  ...z.GPIOPWMActo
-00000f00: 722e 6f6e 5f73 7461 7274 4e63 0200 0000  r.on_startNc....
-00000f10: 0000 0000 0000 0000 0200 0000 0700 0000  ................
-00000f20: c300 0000 73a4 0000 0074 00a0 0164 01a0  ....s....t...d..
-00000f30: 027c 01a1 01a1 0101 007c 0164 0075 0172  .|.......|.d.u.r
-00000f40: 207c 017c 005f 036e 0664 027c 005f 0374   |.|._.n.d.|._.t
-00000f50: 00a0 0164 03a0 027c 006a 03a1 01a1 0101  ...d...|.j......
-00000f60: 0074 04a0 0164 047c 006a 057c 006a 067c  .t...d.|.j.|.j.|
-00000f70: 006a 077c 006a 0366 0416 00a1 0101 007a  .j.|.j.f.......z
-00000f80: 3c7c 006a 0864 0075 0072 7c74 09a0 0a74  <|.j.d.u.r|t...t
-00000f90: 0b7c 006a 0683 0174 0c7c 006a 0783 01a1  .|.j...t.|.j....
-00000fa0: 027c 005f 087c 006a 08a0 0d7c 006a 03a1  .|._.|.j...|.j..
-00000fb0: 0101 0064 057c 005f 0e57 006e 0c01 0001  ...d.|._.W.n....
-00000fc0: 0001 0059 006e 0230 0064 0053 0029 064e  ...Y.n.0.d.S.).N
-00000fd0: 7a13 5057 4d20 4163 746f 7220 506f 7765  z.PWM Actor Powe
-00000fe0: 723a 207b 7d72 3000 0000 7a13 5057 4d20  r: {}r0...z.PWM 
-00000ff0: 4669 6e61 6c20 506f 7765 723a 207b 7d7a  Final Power: {}z
-00001000: 3350 574d 2041 4354 4f52 2025 7320 4f4e  3PWM ACTOR %s ON
-00001010: 202d 2047 5049 4f20 2573 202d 2046 7265   - GPIO %s - Fre
-00001020: 7175 656e 6379 2025 7320 2d20 506f 7765  quency %s - Powe
-00001030: 7220 2573 5429 0f72 5f00 0000 da05 6465  r %sT).r_.....de
-00001040: 6275 67da 0666 6f72 6d61 7472 3300 0000  bug..formatr3...
-00001050: 7247 0000 0072 4900 0000 723f 0000 0072  rG...rI...r?...r
-00001060: 6000 0000 7261 0000 0072 0500 0000 5a03  `...ra...r....Z.
-00001070: 5057 4d72 3200 0000 da05 666c 6f61 74da  PWMr2.....float.
-00001080: 0573 7461 7274 723c 0000 0072 4a00 0000  .startr<...rJ...
-00001090: 7238 0000 0072 3800 0000 7239 0000 0072  r8...r8...r9...r
-000010a0: 4b00 0000 7d00 0000 731a 0000 0000 0110  K...}...s.......
-000010b0: 0108 0108 0206 0212 021e 0102 010a 011a  ................
-000010c0: 010e 010a 0206 017a 0f47 5049 4f50 574d  .......z.GPIOPWM
-000010d0: 4163 746f 722e 6f6e 6301 0000 0000 0000  Actor.onc.......
-000010e0: 0000 0000 0001 0000 0005 0000 00c3 0000  ................
-000010f0: 0073 2c00 0000 7400 a001 6401 7c00 6a02  .s,...t...d.|.j.
-00001100: 7c00 6a03 6602 1600 a101 0100 7c00 6a04  |.j.f.......|.j.
-00001110: a005 6402 a101 0100 6403 7c00 5f06 6400  ..d.....d.|._.d.
-00001120: 5300 2904 4e7a 1b50 574d 2041 4354 4f52  S.).Nz.PWM ACTOR
-00001130: 2025 7320 4f46 4620 2d20 4750 494f 2025   %s OFF - GPIO %
-00001140: 7320 7201 0000 0046 2907 7247 0000 0072  s r....F).rG...r
-00001150: 4800 0000 7249 0000 0072 3f00 0000 7261  H...rI...r?...ra
-00001160: 0000 00da 0f43 6861 6e67 6544 7574 7943  .....ChangeDutyC
-00001170: 7963 6c65 723c 0000 0072 4500 0000 7238  ycler<...rE...r8
-00001180: 0000 0072 3800 0000 7239 0000 0072 4c00  ...r8...r9...rL.
-00001190: 0000 9000 0000 7306 0000 0000 0116 010c  ......s.........
-000011a0: 017a 1047 5049 4f50 574d 4163 746f 722e  .z.GPIOPWMActor.
-000011b0: 6f66 6663 0200 0000 0000 0000 0000 0000  offc............
-000011c0: 0200 0000 0400 0000 c300 0000 7338 0000  ............s8..
-000011d0: 007c 006a 0072 1c7c 006a 0164 016b 0272  .|.j.r.|.j.d.k.r
-000011e0: 1c7c 006a 00a0 027c 01a1 0101 007c 006a  .|.j...|.....|.j
-000011f0: 036a 04a0 057c 006a 067c 01a1 0249 0064  .j...|.j.|...I.d
-00001200: 0048 0001 0064 0053 0029 024e 5429 0772  .H...d.S.).NT).r
-00001210: 6100 0000 723c 0000 0072 6600 0000 7254  a...r<...rf...rT
-00001220: 0000 0072 5500 0000 7256 0000 0072 4900  ...rU...rV...rI.
-00001230: 0000 724a 0000 0072 3800 0000 7238 0000  ..rJ...r8...r8..
-00001240: 0072 3900 0000 7234 0000 0095 0000 0073  .r9...r4.......s
-00001250: 0800 0000 0001 1001 0c01 1801 7a16 4750  ............z.GP
-00001260: 494f 5057 4d41 6374 6f72 2e73 6574 5f70  IOPWMActor.set_p
-00001270: 6f77 6572 6301 0000 0000 0000 0000 0000  owerc...........
-00001280: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-00001290: 0000 7c00 6a00 5300 724d 0000 0072 4e00  ..|.j.S.rM...rN.
-000012a0: 0000 7245 0000 0072 3800 0000 7238 0000  ..rE...r8...r8..
-000012b0: 0072 3900 0000 724f 0000 009b 0000 0073  .r9...rO.......s
-000012c0: 0200 0000 0001 7a16 4750 494f 5057 4d41  ......z.GPIOPWMA
-000012d0: 6374 6f72 2e67 6574 5f73 7461 7465 6301  ctor.get_statec.
-000012e0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-000012f0: 0000 00c3 0000 0073 2000 0000 7c00 6a00  .......s ...|.j.
-00001300: 6401 6b02 721c 7401 a002 6402 a101 4900  d.k.r.t...d...I.
-00001310: 6400 4800 0100 7100 6400 5300 2903 4e54  d.H...q.d.S.).NT
-00001320: 7206 0000 0029 0372 5000 0000 7251 0000  r....).rP...rQ..
-00001330: 0072 5200 0000 7245 0000 0072 3800 0000  .rR...rE...r8...
-00001340: 7238 0000 0072 3900 0000 7253 0000 009e  r8...r9...rS....
-00001350: 0000 0073 0400 0000 0001 0a01 7a10 4750  ...s........z.GP
-00001360: 494f 5057 4d41 6374 6f72 2e72 756e 2901  IOPWMActor.run).
-00001370: 7230 0000 0029 014e 290d 7257 0000 0072  r0...).N).rW...r
-00001380: 5800 0000 7259 0000 0072 5a00 0000 725b  X...rY...rZ...r[
-00001390: 0000 0072 5c00 0000 723a 0000 0072 4600  ...r\...r:...rF.
-000013a0: 0000 724b 0000 0072 4c00 0000 7234 0000  ..rK...rL...r4..
-000013b0: 0072 4f00 0000 7253 0000 0072 3800 0000  .rO...rS...r8...
-000013c0: 7238 0000 0072 3800 0000 7239 0000 0072  r8...r8...r9...r
-000013d0: 5e00 0000 6400 0000 7310 0000 0008 0418  ^...d...s.......
-000013e0: 010c 0908 0b0a 1308 0508 0608 0372 5e00  .............r^.
-000013f0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00001400: 0000 0004 0000 0043 0000 0073 2000 0000  .......C...s ...
-00001410: 7c00 6a00 a001 6401 7402 a102 0100 7c00  |.j...d.t.....|.
-00001420: 6a00 a001 6402 7403 a102 0100 6403 5300  j...d.t.....d.S.
-00001430: 2904 7aa9 0a20 2020 2054 6869 7320 6d65  ).z..    This me
-00001440: 7468 6f64 2069 7320 6361 6c6c 6564 2062  thod is called b
-00001450: 7920 7468 6520 7365 7276 6572 2064 7572  y the server dur
-00001460: 696e 6720 7374 6172 7475 7020 0a20 2020  ing startup .   
-00001470: 2048 6572 6520 796f 7520 6e65 6564 2074   Here you need t
-00001480: 6f20 7265 6769 7374 6572 2079 6f75 7220  o register your 
-00001490: 706c 7567 696e 7320 6174 2074 6865 2073  plugins at the s
-000014a0: 6572 7665 720a 2020 2020 0a20 2020 203a  erver.    .    :
-000014b0: 7061 7261 6d20 6362 7069 3a20 7468 6520  param cbpi: the 
-000014c0: 6362 7069 2063 6f72 6520 0a20 2020 203a  cbpi core .    :
-000014d0: 7265 7475 726e 3a20 0a20 2020 2072 2800  return: .    r(.
-000014e0: 0000 725e 0000 004e 2904 da06 706c 7567  ..r^...N)...plug
-000014f0: 696e da08 7265 6769 7374 6572 7228 0000  in..registerr(..
-00001500: 0072 5e00 0000 2901 7254 0000 0072 3800  .r^...).rT...r8.
-00001510: 0000 7238 0000 0072 3900 0000 7242 0000  ..r8...r9...rB..
-00001520: 00a2 0000 0073 0400 0000 000a 0e01 7242  .....s........rB
-00001530: 0000 0029 1e72 5100 0000 725f 0000 005a  ...).rQ...r_...Z
-00001540: 0d75 6e69 7474 6573 742e 6d6f 636b 7202  .unittest.mockr.
-00001550: 0000 0072 0300 0000 5a08 6362 7069 2e61  ...r....Z.cbpi.a
-00001560: 7069 da09 6765 744c 6f67 6765 7272 5700  pi..getLoggerrW.
-00001570: 0000 7247 0000 005a 0852 5069 2e47 5049  ..rG...Z.RPi.GPI
-00001580: 4f72 0500 0000 da09 4578 6365 7074 696f  Or......Exceptio
-00001590: 6eda 0777 6172 6e69 6e67 5a07 4d6f 636b  n..warningZ.Mock
-000015a0: 5250 69da 076d 6f64 756c 6573 da04 6469  RPi..modules..di
-000015b0: 6374 da07 7061 7463 6865 7272 6500 0000  ct..patcherre...
-000015c0: 5a07 6765 746d 6f64 65da 046d 6f64 65da  Z.getmode..mode.
-000015d0: 0773 6574 6d6f 6465 5a03 4243 4d72 2f00  .setmodeZ.BCMr/.
-000015e0: 0000 725b 0000 00da 0653 656c 6563 74da  ..r[.....Select.
-000015f0: 0943 4250 6941 6374 6f72 7228 0000 0072  .CBPiActorr(...r
-00001600: 5c00 0000 725e 0000 0072 4200 0000 7238  \...r^...rB...r8
-00001610: 0000 0072 3800 0000 7238 0000 0072 3900  ...r8...r8...r9.
-00001620: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001630: 7334 0000 0008 0108 0110 0208 030a 0202  s4..............
-00001640: 0110 010c 010a 0106 0202 0104 fe06 040c  ................
-00001650: 0108 0112 0208 0108 010c 0212 0112 0112  ................
-00001660: fe04 0312 4622 0112 3d                   ....F"..=
+00000140: 6416 6417 8d02 6517 6a18 640a 640b 640c  d.d...e.j.d.d.d.
+00000150: 6702 6418 640e 8d03 6703 8301 4700 6419  g.d.d...g...G.d.
+00000160: 641a 8400 641a 6519 8303 8301 5a1c 641b  d...d.e.....Z.d.
+00000170: 641c 8400 5a1d 6401 5300 291d e900 0000  d...Z.d.S.).....
+00000180: 004e 2902 da09 4d61 6769 634d 6f63 6bda  .N)...MagicMock.
+00000190: 0570 6174 6368 2901 da01 2a7a 2b46 6169  .patch)...*z+Fai
+000001a0: 6c65 6420 746f 206c 6f61 6420 5250 692e  led to load RPi.
+000001b0: 4750 494f 2e20 5573 696e 6720 4d6f 636b  GPIO. Using Mock
+000001c0: 2069 6e73 7465 6164 2902 5a03 5250 697a   instead).Z.RPiz
+000001d0: 0852 5069 2e47 5049 4f7a 0b73 7973 2e6d  .RPi.GPIOz.sys.m
+000001e0: 6f64 756c 6573 da04 4750 494f 291c 7201  odules..GPIO).r.
+000001f0: 0000 00e9 0100 0000 e902 0000 00e9 0300  ................
+00000200: 0000 e904 0000 00e9 0500 0000 e906 0000  ................
+00000210: 00e9 0700 0000 e908 0000 00e9 0900 0000  ................
+00000220: e90a 0000 00e9 0b00 0000 e90c 0000 00e9  ................
+00000230: 0d00 0000 e90e 0000 00e9 0f00 0000 e910  ................
+00000240: 0000 00e9 1100 0000 e912 0000 00e9 1300  ................
+00000250: 0000 e914 0000 00e9 1500 0000 e916 0000  ................
+00000260: 00e9 1700 0000 e918 0000 00e9 1900 0000  ................
+00000270: e91a 0000 00e9 1b00 0000 2902 da05 6c61  ..........)...la
+00000280: 6265 6cda 076f 7074 696f 6e73 da08 496e  bel..options..In
+00000290: 7665 7274 6564 da03 5965 73da 024e 6f7a  verted..Yes..Noz
+000002a0: 264e 6f3a 2041 6374 6976 6520 6f6e 2068  &No: Active on h
+000002b0: 6967 683b 2059 6573 3a20 4163 7469 7665  igh; Yes: Active
+000002c0: 206f 6e20 6c6f 7729 0372 2100 0000 7222   on low).r!...r"
+000002d0: 0000 00da 0b64 6573 6372 6970 7469 6f6e  .....description
+000002e0: da0c 5361 6d70 6c69 6e67 5469 6d65 7207  ..SamplingTimer.
+000002f0: 0000 0072 0a00 0000 7a33 5469 6d65 2069  ...r....z3Time i
+00000300: 6e20 7365 636f 6e64 7320 666f 7220 706f  n seconds for po
+00000310: 7765 7220 6261 7365 2069 6e74 6572 7661  wer base interva
+00000320: 6c20 2844 6566 6175 6c74 3a35 2963 0000  l (Default:5)c..
+00000330: 0000 0000 0000 0000 0000 0000 0000 0700  ................
+00000340: 0000 4000 0000 736a 0000 0065 005a 0164  ..@...sj...e.Z.d
+00000350: 005a 0265 0364 0165 046a 0564 0264 0364  .Z.e.d.e.j.d.d.d
+00000360: 0464 058d 0367 0164 068d 0264 1964 0864  .d...g.d...d.d.d
+00000370: 0984 0183 015a 0664 0a64 0b84 005a 0764  .....Z.d.d...Z.d
+00000380: 0c64 0d84 005a 0864 1a64 0f64 1084 015a  .d...Z.d.d.d...Z
+00000390: 0964 1164 1284 005a 0a64 1364 1484 005a  .d.d...Z.d.d...Z
+000003a0: 0b64 1564 1684 005a 0c64 1764 1884 005a  .d.d...Z.d.d...Z
+000003b0: 0d64 0e53 0029 1bda 0947 5049 4f41 6374  .d.S.)...GPIOAct
+000003c0: 6f72 fa09 5365 7420 506f 7765 72da 0550  or..Set Power..P
+000003d0: 6f77 6572 54fa 1550 6f77 6572 2053 6574  owerT..Power Set
+000003e0: 7469 6e67 205b 302d 3130 305d a903 7221  ting [0-100]..r!
+000003f0: 0000 00da 0c63 6f6e 6669 6775 7261 626c  .....configurabl
+00000400: 6572 2600 0000 a901 da0a 7061 7261 6d65  er&.......parame
+00000410: 7465 7273 e964 0000 0063 0200 0000 0000  ters.d...c......
+00000420: 0000 0000 0000 0300 0000 0300 0000 cb00  ................
+00000430: 0000 7340 0000 0074 007c 0183 017c 005f  ..s@...t.|...|._
+00000440: 017c 006a 0164 016b 0072 1a64 017c 005f  .|.j.d.k.r.d.|._
+00000450: 017c 006a 0164 026b 0472 2a64 027c 005f  .|.j.d.k.r*d.|._
+00000460: 017c 00a0 027c 006a 01a1 0149 0064 0048  .|...|.j...I.d.H
+00000470: 0001 0064 0053 00a9 034e 7201 0000 0072  ...d.S...Nr....r
+00000480: 3000 0000 2903 da03 696e 74da 0570 6f77  0...)...int..pow
+00000490: 6572 da09 7365 745f 706f 7765 72a9 03da  er..set_power...
+000004a0: 0473 656c 6672 2a00 0000 da06 6b77 6172  .selfr*.....kwar
+000004b0: 6773 a900 7238 0000 00fa 5863 3a5c 7573  gs..r8....Xc:\us
+000004c0: 6572 735c 616c 6578 616e 6465 725c 646f  ers\alexander\do
+000004d0: 776e 6c6f 6164 735c 6372 6166 7462 6565  wnloads\craftbee
+000004e0: 7270 6934 5f61 766f 6c6c 6b6f 7066 5c63  rpi4_avollkopf\c
+000004f0: 6270 695c 6578 7465 6e73 696f 6e5c 6770  bpi\extension\gp
+00000500: 696f 6163 746f 725c 5f5f 696e 6974 5f5f  ioactor\__init__
+00000510: 2e70 79da 0873 6574 706f 7765 7221 0000  .py..setpower!..
+00000520: 0073 0c00 0000 0002 0a01 0a01 0601 0a01  .s..............
+00000530: 0601 7a12 4750 494f 4163 746f 722e 7365  ..z.GPIOActor.se
+00000540: 7470 6f77 6572 6302 0000 0000 0000 0000  tpowerc.........
+00000550: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00000560: 3800 0000 7c01 6401 6b02 721a 7c00 6a00  8...|.d.k.r.|.j.
+00000570: 6402 6b02 7216 6401 5300 6403 5300 7c01  d.k.r.d.S.d.S.|.
+00000580: 6403 6b02 7234 7c00 6a00 6402 6b02 7230  d.k.r4|.j.d.k.r0
+00000590: 6403 5300 6401 5300 6400 5300 2904 4e72  d.S.d.S.d.S.).Nr
+000005a0: 0600 0000 4672 0100 0000 2901 da08 696e  ....Fr....)...in
+000005b0: 7665 7274 6564 2902 7236 0000 00da 0573  verted).r6.....s
+000005c0: 7461 7465 7238 0000 0072 3800 0000 7239  tater8...r8...r9
+000005d0: 0000 00da 0e67 6574 5f47 5049 4f5f 7374  .....get_GPIO_st
+000005e0: 6174 652a 0000 0073 0800 0000 0002 0801  ate*...s........
+000005f0: 1202 0801 7a18 4750 494f 4163 746f 722e  ....z.GPIOActor.
+00000600: 6765 745f 4750 494f 5f73 7461 7465 6301  get_GPIO_statec.
+00000610: 0000 0000 0000 0000 0000 0001 0000 0006  ................
+00000620: 0000 00c3 0000 0073 6e00 0000 6400 7c00  .......sn...d.|.
+00000630: 5f00 7c00 6a01 6a02 7c00 5f03 7c00 6a01  _.|.j.j.|._.|.j.
+00000640: a004 6401 6402 a102 6403 6b02 7226 6404  ..d.d...d.k.r&d.
+00000650: 6e02 6405 7c00 5f05 7406 7c00 6a01 a004  n.d.|._.t.|.j...
+00000660: 6406 6407 a102 8301 7c00 5f07 7402 a008  d.d.....|._.t...
+00000670: 7c00 6a03 7402 6a09 a102 0100 7402 a00a  |.j.t.j.....t...
+00000680: 7c00 6a03 7c00 a00b 6408 a101 a102 0100  |.j.|...d.......
+00000690: 6405 7c00 5f0c 6400 5300 2909 4e72 2300  d.|._.d.S.).Nr#.
+000006a0: 0000 7225 0000 0072 2400 0000 5446 7227  ..r%...r$...TFr'
+000006b0: 0000 0072 0a00 0000 7201 0000 0029 0d72  ...r....r....).r
+000006c0: 3300 0000 da05 7072 6f70 7372 0500 0000  3.....propsr....
+000006d0: da04 6770 696f da03 6765 7472 3b00 0000  ..gpio..getr;...
+000006e0: 7232 0000 00da 0a73 616d 706c 6554 696d  r2.....sampleTim
+000006f0: 65da 0573 6574 7570 da03 4f55 54da 066f  e..setup..OUT..o
+00000700: 7574 7075 7472 3d00 0000 723c 0000 00a9  utputr=...r<....
+00000710: 0172 3600 0000 7238 0000 0072 3800 0000  .r6...r8...r8...
+00000720: 7239 0000 00da 086f 6e5f 7374 6172 7432  r9.....on_start2
+00000730: 0000 0073 0e00 0000 0001 0601 0a01 1c01  ...s............
+00000740: 1401 1001 1401 7a12 4750 494f 4163 746f  ......z.GPIOActo
+00000750: 722e 6f6e 5f73 7461 7274 4e63 0200 0000  r.on_startNc....
+00000760: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00000770: c300 0000 734a 0000 007c 0164 0075 0172  ....sJ...|.d.u.r
+00000780: 107c 017c 005f 006e 0664 017c 005f 0074  .|.|._.n.d.|._.t
+00000790: 01a0 0264 027c 006a 037c 006a 0466 0216  ...d.|.j.|.j.f..
+000007a0: 00a1 0101 0074 05a0 067c 006a 047c 00a0  .....t...|.j.|..
+000007b0: 0764 03a1 01a1 0201 0064 047c 005f 0864  .d.......d.|._.d
+000007c0: 0053 0029 054e 7230 0000 007a 1641 4354  .S.).Nr0...z.ACT
+000007d0: 4f52 2025 7320 4f4e 202d 2047 5049 4f20  OR %s ON - GPIO 
+000007e0: 2573 2072 0600 0000 5429 0972 3300 0000  %s r....T).r3...
+000007f0: da06 6c6f 6767 6572 da04 696e 666f da02  ..logger..info..
+00000800: 6964 723f 0000 0072 0500 0000 7244 0000  idr?...r....rD..
+00000810: 0072 3d00 0000 723c 0000 00a9 0272 3600  .r=...r<.....r6.
+00000820: 0000 7233 0000 0072 3800 0000 7238 0000  ..r3...r8...r8..
+00000830: 0072 3900 0000 da02 6f6e 3b00 0000 730c  .r9.....on;...s.
+00000840: 0000 0000 0108 0108 0206 0316 0114 017a  ...............z
+00000850: 0c47 5049 4f41 6374 6f72 2e6f 6e63 0100  .GPIOActor.onc..
+00000860: 0000 0000 0000 0000 0000 0100 0000 0600  ................
+00000870: 0000 c300 0000 7334 0000 0074 00a0 0164  ......s4...t...d
+00000880: 017c 006a 027c 006a 0366 0216 00a1 0101  .|.j.|.j.f......
+00000890: 0074 04a0 057c 006a 037c 00a0 0664 02a1  .t...|.j.|...d..
+000008a0: 01a1 0201 0064 037c 005f 0764 0053 0029  .....d.|._.d.S.)
+000008b0: 044e 7a17 4143 544f 5220 2573 204f 4646  .Nz.ACTOR %s OFF
+000008c0: 202d 2047 5049 4f20 2573 2072 0100 0000   - GPIO %s r....
+000008d0: 4629 0872 4700 0000 7248 0000 0072 4900  F).rG...rH...rI.
+000008e0: 0000 723f 0000 0072 0500 0000 7244 0000  ..r?...r....rD..
+000008f0: 0072 3d00 0000 723c 0000 0072 4500 0000  .r=...r<...rE...
+00000900: 7238 0000 0072 3800 0000 7239 0000 00da  r8...r8...r9....
+00000910: 036f 6666 4600 0000 7306 0000 0000 0116  .offF...s.......
+00000920: 0114 017a 0d47 5049 4f41 6374 6f72 2e6f  ...z.GPIOActor.o
+00000930: 6666 6301 0000 0000 0000 0000 0000 0001  ffc.............
+00000940: 0000 0001 0000 0043 0000 0073 0600 0000  .......C...s....
+00000950: 7c00 6a00 5300 a901 4ea9 0172 3c00 0000  |.j.S...N..r<...
+00000960: 7245 0000 0072 3800 0000 7238 0000 0072  rE...r8...r8...r
+00000970: 3900 0000 da09 6765 745f 7374 6174 654b  9.....get_stateK
+00000980: 0000 0073 0200 0000 0001 7a13 4750 494f  ...s......z.GPIO
+00000990: 4163 746f 722e 6765 745f 7374 6174 6563  Actor.get_statec
+000009a0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000009b0: 0600 0000 c300 0000 739e 0000 007c 006a  ........s....|.j
+000009c0: 0064 016b 0272 9a7c 006a 0164 016b 0272  .d.k.r.|.j.d.k.r
+000009d0: 887c 006a 027c 006a 0364 021b 0014 007d  .|.j.|.j.d.....}
+000009e0: 017c 006a 027c 0118 007d 027c 0164 036b  .|.j.|...}.|.d.k
+000009f0: 0472 5a74 04a0 057c 006a 067c 00a0 0764  .rZt...|.j.|...d
+00000a00: 04a1 01a1 0201 0074 08a0 097c 01a1 0149  .......t...|...I
+00000a10: 0064 0048 0001 007c 0264 036b 0472 9874  .d.H...|.d.k.r.t
+00000a20: 04a0 057c 006a 067c 00a0 0764 03a1 01a1  ...|.j.|...d....
+00000a30: 0201 0074 08a0 097c 02a1 0149 0064 0048  ...t...|...I.d.H
+00000a40: 0001 0071 0074 08a0 0964 04a1 0149 0064  ...q.t...d...I.d
+00000a50: 0048 0001 0071 0064 0053 0029 054e 5472  .H...q.d.S.).NTr
+00000a60: 3000 0000 7201 0000 0072 0600 0000 290a  0...r....r....).
+00000a70: da07 7275 6e6e 696e 6772 3c00 0000 7241  ..runningr<...rA
+00000a80: 0000 0072 3300 0000 7205 0000 0072 4400  ...r3...r....rD.
+00000a90: 0000 723f 0000 0072 3d00 0000 da07 6173  ..r?...r=.....as
+00000aa0: 796e 6369 6fda 0573 6c65 6570 2903 7236  yncio..sleep).r6
+00000ab0: 0000 005a 0c68 6561 7469 6e67 5f74 696d  ...Z.heating_tim
+00000ac0: 655a 0977 6169 745f 7469 6d65 7238 0000  eZ.wait_timer8..
+00000ad0: 0072 3800 0000 7239 0000 00da 0372 756e  .r8...r9.....run
+00000ae0: 4e00 0000 7316 0000 0000 010a 010a 0110  N...s...........
+00000af0: 010a 0108 0214 0110 0108 0214 0112 027a  ...............z
+00000b00: 0d47 5049 4f41 6374 6f72 2e72 756e 6302  .GPIOActor.runc.
+00000b10: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00000b20: 0000 00c3 0000 0073 2200 0000 7c01 7c00  .......s"...|.|.
+00000b30: 5f00 7c00 6a01 6a02 a003 7c00 6a04 7c01  _.|.j.j...|.j.|.
+00000b40: a102 4900 6400 4800 0100 6400 5300 724d  ..I.d.H...d.S.rM
+00000b50: 0000 0029 0572 3300 0000 da04 6362 7069  ...).r3.....cbpi
+00000b60: da05 6163 746f 72da 0c61 6374 6f72 5f75  ..actor..actor_u
+00000b70: 7064 6174 6572 4900 0000 724a 0000 0072  pdaterI...rJ...r
+00000b80: 3800 0000 7238 0000 0072 3900 0000 7234  8...r8...r9...r4
+00000b90: 0000 005e 0000 0073 0600 0000 0001 0601  ...^...s........
+00000ba0: 1801 7a13 4750 494f 4163 746f 722e 7365  ..z.GPIOActor.se
+00000bb0: 745f 706f 7765 7229 0172 3000 0000 2901  t_power).r0...).
+00000bc0: 4e29 0eda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000bd0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000be0: 6c6e 616d 655f 5fda 0661 6374 696f 6eda  lname__..action.
+00000bf0: 0850 726f 7065 7274 79da 064e 756d 6265  .Property..Numbe
+00000c00: 7272 3a00 0000 723d 0000 0072 4600 0000  rr:...r=...rF...
+00000c10: 724b 0000 0072 4c00 0000 724f 0000 0072  rK...rL...rO...r
+00000c20: 5300 0000 7234 0000 0072 3800 0000 7238  S...r4...r8...r8
+00000c30: 0000 0072 3800 0000 7239 0000 0072 2800  ...r8...r9...r(.
+00000c40: 0000 1b00 0000 7312 0000 0008 0618 010c  ......s.........
+00000c50: 0808 0808 090a 0b08 0508 0308 1072 2800  .............r(.
+00000c60: 0000 da09 4672 6571 7565 6e63 7954 2902  ....FrequencyT).
+00000c70: 7221 0000 0072 2d00 0000 7a3c 496e 7665  r!...r-...z<Inve
+00000c80: 7274 7320 5057 4d20 6c6f 6164 2069 6620  rts PWM load if 
+00000c90: 7365 7420 746f 2079 6573 2028 652e 672e  set to yes (e.g.
+00000ca0: 2039 3025 203d 2031 3025 292e 2044 6566   90% = 10%). Def
+00000cb0: 6175 6c74 3a20 4e6f 6300 0000 0000 0000  ault: Noc.......
+00000cc0: 0000 0000 0000 0000 0007 0000 0040 0000  .............@..
+00000cd0: 0073 6200 0000 6500 5a01 6400 5a02 6503  .sb...e.Z.d.Z.e.
+00000ce0: 6401 6504 6a05 6402 6403 6404 6405 8d03  d.e.j.d.d.d.d...
+00000cf0: 6701 6406 8d02 6417 6408 6409 8401 8301  g.d...d.d.d.....
+00000d00: 5a06 640a 640b 8400 5a07 6418 640d 640e  Z.d.d...Z.d.d.d.
+00000d10: 8401 5a08 640f 6410 8400 5a09 6411 6412  ..Z.d.d...Z.d.d.
+00000d20: 8400 5a0a 6413 6414 8400 5a0b 6415 6416  ..Z.d.d...Z.d.d.
+00000d30: 8400 5a0c 640c 5300 2919 da0c 4750 494f  ..Z.d.S.)...GPIO
+00000d40: 5057 4d41 6374 6f72 7229 0000 0072 2a00  PWMActorr)...r*.
+00000d50: 0000 5472 2b00 0000 722c 0000 0072 2e00  ..Tr+...r,...r..
+00000d60: 0000 7230 0000 0063 0200 0000 0000 0000  ..r0...c........
+00000d70: 0000 0000 0300 0000 0300 0000 cb00 0000  ................
+00000d80: 734a 0000 0074 00a0 017c 01a1 0101 0074  sJ...t...|.....t
+00000d90: 027c 0183 017c 005f 037c 006a 0364 016b  .|...|._.|.j.d.k
+00000da0: 0072 2464 017c 005f 037c 006a 0364 026b  .r$d.|._.|.j.d.k
+00000db0: 0472 3464 027c 005f 037c 00a0 047c 006a  .r4d.|._.|...|.j
+00000dc0: 03a1 0149 0064 0048 0001 0064 0053 0072  ...I.d.H...d.S.r
+00000dd0: 3100 0000 2905 da07 6c6f 6767 696e 6772  1...)...loggingr
+00000de0: 4800 0000 7232 0000 0072 3300 0000 7234  H...r2...r3...r4
+00000df0: 0000 0072 3500 0000 7238 0000 0072 3800  ...r5...r8...r8.
+00000e00: 0000 7239 0000 0072 3a00 0000 6a00 0000  ..r9...r:...j...
+00000e10: 730e 0000 0000 020a 010a 010a 0106 010a  s...............
+00000e20: 0106 017a 1547 5049 4f50 574d 4163 746f  ...z.GPIOPWMActo
+00000e30: 722e 7365 7470 6f77 6572 6301 0000 0000  r.setpowerc.....
+00000e40: 0000 0000 0000 0001 0000 0004 0000 00c3  ................
+00000e50: 0000 0073 8800 0000 7c00 6a00 a001 6401  ...s....|.j...d.
+00000e60: 6400 a102 7c00 5f02 7c00 6a00 a001 6402  d...|._.|.j...d.
+00000e70: 6403 a102 7c00 5f03 7c00 6a00 a001 6404  d...|._.|.j...d.
+00000e80: 6405 a102 7c00 5f04 7c00 6a02 6400 7501  d...|._.|.j.d.u.
+00000e90: 7272 7405 a006 7c00 6a02 7405 6a07 a102  rrt...|.j.t.j...
+00000ea0: 0100 7c00 6a03 6403 6b02 7264 7405 a008  ..|.j.d.k.rdt...
+00000eb0: 7c00 6a02 6406 a102 0100 6e0e 7405 a008  |.j.d.....n.t...
+00000ec0: 7c00 6a02 6407 a102 0100 6408 7c00 5f09  |.j.d.....d.|._.
+00000ed0: 6400 7c00 5f0a 6400 7c00 5f0b 6400 5300  d.|._.d.|._.d.S.
+00000ee0: 2909 4e72 0500 0000 7223 0000 0072 2500  ).Nr....r#...r%.
+00000ef0: 0000 725d 0000 0067 0000 0000 0000 e03f  ..r]...g.......?
+00000f00: 7201 0000 0072 0600 0000 4629 0c72 3e00  r....r....F).r>.
+00000f10: 0000 7240 0000 0072 3f00 0000 723b 0000  ..r@...r?...r;..
+00000f20: 00da 0966 7265 7175 656e 6379 7205 0000  ...frequencyr...
+00000f30: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
+00000f40: 723c 0000 0072 3300 0000 da01 7072 4500  r<...r3.....prE.
+00000f50: 0000 7238 0000 0072 3800 0000 7239 0000  ..r8...r8...r9..
+00000f60: 0072 4600 0000 7400 0000 7318 0000 0000  .rF...t...s.....
+00000f70: 0110 0110 0110 010a 0110 010a 0110 020e  ................
+00000f80: 0106 0106 0106 017a 1547 5049 4f50 574d  .......z.GPIOPWM
+00000f90: 4163 746f 722e 6f6e 5f73 7461 7274 4e63  Actor.on_startNc
+00000fa0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000fb0: 0700 0000 c300 0000 73c2 0000 0074 00a0  ........s....t..
+00000fc0: 0164 01a0 027c 01a1 01a1 0101 007c 0164  .d...|.......|.d
+00000fd0: 0075 0172 207c 017c 005f 036e 0664 027c  .u.r |.|._.n.d.|
+00000fe0: 005f 0374 00a0 0164 03a0 027c 006a 03a1  ._.t...d...|.j..
+00000ff0: 01a1 0101 0074 04a0 0164 047c 006a 057c  .....t...d.|.j.|
+00001000: 006a 067c 006a 077c 006a 0366 0416 00a1  .j.|.j.|.j.f....
+00001010: 0101 007a 5a7c 006a 0864 0075 0072 7c74  ...zZ|.j.d.u.r|t
+00001020: 09a0 0a74 0b7c 006a 0683 0174 0c7c 006a  ...t.|.j...t.|.j
+00001030: 0783 01a1 027c 005f 087c 006a 0d64 056b  .....|._.|.j.d.k
+00001040: 0272 967c 006a 08a0 0e7c 006a 03a1 0101  .r.|.j...|.j....
+00001050: 006e 127c 006a 08a0 0e64 027c 006a 0318  .n.|.j...d.|.j..
+00001060: 00a1 0101 0064 067c 005f 0f57 006e 0c01  .....d.|._.W.n..
+00001070: 0001 0001 0059 006e 0230 0064 0053 0029  .....Y.n.0.d.S.)
+00001080: 074e 7a13 5057 4d20 4163 746f 7220 506f  .Nz.PWM Actor Po
+00001090: 7765 723a 207b 7d72 3000 0000 7a13 5057  wer: {}r0...z.PW
+000010a0: 4d20 4669 6e61 6c20 506f 7765 723a 207b  M Final Power: {
+000010b0: 7d7a 3350 574d 2041 4354 4f52 2025 7320  }z3PWM ACTOR %s 
+000010c0: 4f4e 202d 2047 5049 4f20 2573 202d 2046  ON - GPIO %s - F
+000010d0: 7265 7175 656e 6379 2025 7320 2d20 506f  requency %s - Po
+000010e0: 7765 7220 2573 7225 0000 0054 2910 725f  wer %sr%...T).r_
+000010f0: 0000 00da 0564 6562 7567 da06 666f 726d  .....debug..form
+00001100: 6174 7233 0000 0072 4700 0000 7249 0000  atr3...rG...rI..
+00001110: 0072 3f00 0000 7260 0000 0072 6100 0000  .r?...r`...ra...
+00001120: 7205 0000 005a 0350 574d 7232 0000 00da  r....Z.PWMr2....
+00001130: 0566 6c6f 6174 723b 0000 00da 0573 7461  .floatr;.....sta
+00001140: 7274 723c 0000 0072 4a00 0000 7238 0000  rtr<...rJ...r8..
+00001150: 0072 3800 0000 7239 0000 0072 4b00 0000  .r8...r9...rK...
+00001160: 8300 0000 731e 0000 0000 0110 0108 0108  ....s...........
+00001170: 0206 0212 021e 0102 010a 011a 010a 0110  ................
+00001180: 0212 010a 0206 017a 0f47 5049 4f50 574d  .......z.GPIOPWM
+00001190: 4163 746f 722e 6f6e 6301 0000 0000 0000  Actor.onc.......
+000011a0: 0000 0000 0001 0000 0005 0000 00c3 0000  ................
+000011b0: 0073 4400 0000 7400 a001 6401 7c00 6a02  .sD...t...d.|.j.
+000011c0: 7c00 6a03 6602 1600 a101 0100 7c00 6a04  |.j.f.......|.j.
+000011d0: 6402 6b02 722e 7c00 6a05 a006 6403 a101  d.k.r.|.j...d...
+000011e0: 0100 6e0c 7c00 6a05 a006 6404 a101 0100  ..n.|.j...d.....
+000011f0: 6405 7c00 5f07 6400 5300 2906 4e7a 1b50  d.|._.d.S.).Nz.P
+00001200: 574d 2041 4354 4f52 2025 7320 4f46 4620  WM ACTOR %s OFF 
+00001210: 2d20 4750 494f 2025 7320 7225 0000 0072  - GPIO %s r%...r
+00001220: 0100 0000 7230 0000 0046 2908 7247 0000  ....r0...F).rG..
+00001230: 0072 4800 0000 7249 0000 0072 3f00 0000  .rH...rI...r?...
+00001240: 723b 0000 0072 6100 0000 da0f 4368 616e  r;...ra.....Chan
+00001250: 6765 4475 7479 4379 636c 6572 3c00 0000  geDutyCycler<...
+00001260: 7245 0000 0072 3800 0000 7238 0000 0072  rE...r8...r8...r
+00001270: 3900 0000 724c 0000 0099 0000 0073 0a00  9...rL.......s..
+00001280: 0000 0001 1601 0a01 0e02 0c02 7a10 4750  ............z.GP
+00001290: 494f 5057 4d41 6374 6f72 2e6f 6666 6302  IOPWMActor.offc.
+000012a0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+000012b0: 0000 00c3 0000 0073 5400 0000 7c00 6a00  .......sT...|.j.
+000012c0: 7238 7c00 6a01 6401 6b02 7238 7c00 6a02  r8|.j.d.k.r8|.j.
+000012d0: 6402 6b02 7228 7c00 6a00 a003 7c01 a101  d.k.r(|.j...|...
+000012e0: 0100 6e10 7c00 6a00 a003 6403 7c01 1800  ..n.|.j...d.|...
+000012f0: a101 0100 7c00 6a04 6a05 a006 7c00 6a07  ....|.j.j...|.j.
+00001300: 7c01 a102 4900 6400 4800 0100 6400 5300  |...I.d.H...d.S.
+00001310: 2904 4e54 7225 0000 0072 3000 0000 2908  ).NTr%...r0...).
+00001320: 7261 0000 0072 3c00 0000 723b 0000 0072  ra...r<...r;...r
+00001330: 6600 0000 7254 0000 0072 5500 0000 7256  f...rT...rU...rV
+00001340: 0000 0072 4900 0000 724a 0000 0072 3800  ...rI...rJ...r8.
+00001350: 0000 7238 0000 0072 3900 0000 7234 0000  ..r8...r9...r4..
+00001360: 00a2 0000 0073 0c00 0000 0001 1001 0a01  .....s..........
+00001370: 0e02 1001 1801 7a16 4750 494f 5057 4d41  ......z.GPIOPWMA
+00001380: 6374 6f72 2e73 6574 5f70 6f77 6572 6301  ctor.set_powerc.
+00001390: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+000013a0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
+000013b0: 5300 724d 0000 0072 4e00 0000 7245 0000  S.rM...rN...rE..
+000013c0: 0072 3800 0000 7238 0000 0072 3900 0000  .r8...r8...r9...
+000013d0: 724f 0000 00ab 0000 0073 0200 0000 0001  rO.......s......
+000013e0: 7a16 4750 494f 5057 4d41 6374 6f72 2e67  z.GPIOPWMActor.g
+000013f0: 6574 5f73 7461 7465 6301 0000 0000 0000  et_statec.......
+00001400: 0000 0000 0001 0000 0003 0000 00c3 0000  ................
+00001410: 0073 2000 0000 7c00 6a00 6401 6b02 721c  .s ...|.j.d.k.r.
+00001420: 7401 a002 6402 a101 4900 6400 4800 0100  t...d...I.d.H...
+00001430: 7100 6400 5300 2903 4e54 7206 0000 0029  q.d.S.).NTr....)
+00001440: 0372 5000 0000 7251 0000 0072 5200 0000  .rP...rQ...rR...
+00001450: 7245 0000 0072 3800 0000 7238 0000 0072  rE...r8...r8...r
+00001460: 3900 0000 7253 0000 00ae 0000 0073 0400  9...rS.......s..
+00001470: 0000 0001 0a01 7a10 4750 494f 5057 4d41  ......z.GPIOPWMA
+00001480: 6374 6f72 2e72 756e 2901 7230 0000 0029  ctor.run).r0...)
+00001490: 014e 290d 7257 0000 0072 5800 0000 7259  .N).rW...rX...rY
+000014a0: 0000 0072 5a00 0000 725b 0000 0072 5c00  ...rZ...r[...r\.
+000014b0: 0000 723a 0000 0072 4600 0000 724b 0000  ..r:...rF...rK..
+000014c0: 0072 4c00 0000 7234 0000 0072 4f00 0000  .rL...r4...rO...
+000014d0: 7253 0000 0072 3800 0000 7238 0000 0072  rS...r8...r8...r
+000014e0: 3800 0000 7239 0000 0072 5e00 0000 6400  8...r9...r^...d.
+000014f0: 0000 7310 0000 0008 0618 010c 0908 0f0a  ..s.............
+00001500: 1608 0908 0908 0372 5e00 0000 6301 0000  .......r^...c...
+00001510: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00001520: 0043 0000 0073 2000 0000 7c00 6a00 a001  .C...s ...|.j...
+00001530: 6401 7402 a102 0100 7c00 6a00 a001 6402  d.t.....|.j...d.
+00001540: 7403 a102 0100 6403 5300 2904 7aa9 0a20  t.....d.S.).z.. 
+00001550: 2020 2054 6869 7320 6d65 7468 6f64 2069     This method i
+00001560: 7320 6361 6c6c 6564 2062 7920 7468 6520  s called by the 
+00001570: 7365 7276 6572 2064 7572 696e 6720 7374  server during st
+00001580: 6172 7475 7020 0a20 2020 2048 6572 6520  artup .    Here 
+00001590: 796f 7520 6e65 6564 2074 6f20 7265 6769  you need to regi
+000015a0: 7374 6572 2079 6f75 7220 706c 7567 696e  ster your plugin
+000015b0: 7320 6174 2074 6865 2073 6572 7665 720a  s at the server.
+000015c0: 2020 2020 0a20 2020 203a 7061 7261 6d20      .    :param 
+000015d0: 6362 7069 3a20 7468 6520 6362 7069 2063  cbpi: the cbpi c
+000015e0: 6f72 6520 0a20 2020 203a 7265 7475 726e  ore .    :return
+000015f0: 3a20 0a20 2020 2072 2800 0000 725e 0000  : .    r(...r^..
+00001600: 004e 2904 da06 706c 7567 696e da08 7265  .N)...plugin..re
+00001610: 6769 7374 6572 7228 0000 0072 5e00 0000  gisterr(...r^...
+00001620: 2901 7254 0000 0072 3800 0000 7238 0000  ).rT...r8...r8..
+00001630: 0072 3900 0000 7242 0000 00b2 0000 0073  .r9...rB.......s
+00001640: 0400 0000 000a 0e01 7242 0000 0029 1e72  ........rB...).r
+00001650: 5100 0000 725f 0000 005a 0d75 6e69 7474  Q...r_...Z.unitt
+00001660: 6573 742e 6d6f 636b 7202 0000 0072 0300  est.mockr....r..
+00001670: 0000 5a08 6362 7069 2e61 7069 da09 6765  ..Z.cbpi.api..ge
+00001680: 744c 6f67 6765 7272 5700 0000 7247 0000  tLoggerrW...rG..
+00001690: 005a 0852 5069 2e47 5049 4f72 0500 0000  .Z.RPi.GPIOr....
+000016a0: da09 4578 6365 7074 696f 6eda 0777 6172  ..Exception..war
+000016b0: 6e69 6e67 5a07 4d6f 636b 5250 69da 076d  ningZ.MockRPi..m
+000016c0: 6f64 756c 6573 da04 6469 6374 da07 7061  odules..dict..pa
+000016d0: 7463 6865 7272 6500 0000 5a07 6765 746d  tcherre...Z.getm
+000016e0: 6f64 65da 046d 6f64 65da 0773 6574 6d6f  ode..mode..setmo
+000016f0: 6465 5a03 4243 4d72 2f00 0000 725b 0000  deZ.BCMr/...r[..
+00001700: 00da 0653 656c 6563 74da 0943 4250 6941  ...Select..CBPiA
+00001710: 6374 6f72 7228 0000 0072 5c00 0000 725e  ctorr(...r\...r^
+00001720: 0000 0072 4200 0000 7238 0000 0072 3800  ...rB...r8...r8.
+00001730: 0000 7238 0000 0072 3900 0000 da08 3c6d  ..r8...r9.....<m
+00001740: 6f64 756c 653e 0100 0000 733a 0000 0008  odule>....s:....
+00001750: 0108 0110 0208 030a 0202 0110 010c 010a  ................
+00001760: 0106 0202 0104 fe06 040c 0108 0112 0208  ................
+00001770: 0108 010c 0212 0112 0112 fe04 0312 4612  ..............F.
+00001780: 010c 0112 fe04 0312 4b                   ........K
```

### Comparing `cbpi4-4.3.2/cbpi/extension/httpsensor/__init__.py` & `cbpi4-4.4.0/cbpi/extension/httpsensor/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/httpsensor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/httpsensor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/httpsensor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/httpsensor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/httpsensor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/httpsensor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/httpsensor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/httpsensor/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/hysteresis/__init__.py` & `cbpi4-4.4.0/cbpi/extension/hysteresis/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/hysteresis/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/hysteresis/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/hysteresis/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/hysteresis/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/hysteresis/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/hysteresis/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/hysteresis/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/hysteresis/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mashstep/__init__.py` & `cbpi4-4.4.0/cbpi/extension/mashstep/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mashstep/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/mashstep/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mashstep/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/mashstep/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mashstep/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/mashstep/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mashstep/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/mashstep/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__init__.py` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/generic_mqtt_actor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/mqtt_actor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/__pycache__/tasmota_mqtt_actor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/generic_mqtt_actor.py` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/generic_mqtt_actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_actor/mqtt_actor.py` & `cbpi4-4.4.0/cbpi/extension/mqtt_actor/mqtt_actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__init__.py` & `cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def __init__(self, cbpi, id, props):
         super(MQTTSensor, self).__init__(cbpi, id, props)
         self.Topic = self.props.get("Topic", None)
         self.payload_text = self.props.get("PayloadDictionary", None)
         if self.payload_text != None:
             self.payload_text = self.payload_text.split('.')
-        self.mqtt_task = self.cbpi.satellite.subcribe(self.Topic, self.on_message)
+        self.subscribed = self.cbpi.satellite.subscribe(self.Topic, self.on_message)
         self.value: float = 999
         self.timeout=int(self.props.get("Timeout", 60))
         self.starttime = time.time()
         self.notificationsend = False
         self.nextchecktime=self.starttime+self.timeout
         self.lastdata=time.time()
         self.lastlog=0
@@ -51,15 +51,15 @@
 
     async def message(self):
         target_timestring= datetime.fromtimestamp(self.lastdata)
         self.cbpi.notify("MQTTSensor Timeout", "Sensor '" + str(self.sensor.name) + "' did not respond. Last data received: "+target_timestring.strftime("%D %H:%M"), NotificationType.WARNING, action=[NotificationAction("OK", self.Confirm)])
         pass
 
     async def on_message(self, message):
-        val = json.loads(message)
+        val = json.loads(message.payload.decode())
         try:
             if self.payload_text is not None:
                 for key in self.payload_text:
                     val = val.get(key, None)
 
             if isinstance(val, (int, float, str)):
                 self.value = float(val)
@@ -126,25 +126,16 @@
                     self.notificationsend=True
             await asyncio.sleep(1)
 
     def get_state(self):
         return dict(value=self.value)
 
     async def on_stop(self):
-        was_cancelled=False
-        if not self.mqtt_task.done():
-            logging.info("Task not done -> cancelling")
-            was_cancelled = self.mqtt_task.cancel()
-        try:            
-            logging.info("Trying to call cancelled task")
-            await self.mqtt_task
-        except asyncio.CancelledError:
-            logging.info("Task has been Cancelled")
-            pass
-        logging.info("Task cancelled: {}".format(was_cancelled))
+        self.subscribed = self.cbpi.satellite.unsubscribe(self.Topic, self.on_message)
+
 
 def setup(cbpi):
     '''
     This method is called by the server during startup
     Here you need to register your plugins at the server
 
     :param cbpi: the cbpi core
```

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_sensor/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 28 04:55:57 2023 UTC, .py size: 7318 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5d73 2264 961c 0000  a.......]s"d....
+00000000: 610d 0d0a 0000 0000 c50f de65 291b 0000  a..........e)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c04  m.Z.m.Z...d.d.l.
 00000060: 5400 6400 6401 6c08 5a08 6400 6401 6c09  T.d.d.l.Z.d.d.l.
 00000070: 5a09 6400 6401 6c0a 5a0a 6400 6405 6c0b  Z.d.d.l.Z.d.d.l.
@@ -100,258 +100,244 @@
 00000630: 7474 6c65 2064 6566 696e 6564 2066 6f72  ttle defined for
 00000640: 2072 6564 7563 6564 206c 6f67 6769 6e67   reduced logging
 00000650: 2eda 024f 4ba9 01da 0661 6374 696f 6e29  ...OK....action)
 00000660: 24da 0573 7570 6572 7216 0000 00da 085f  $..superr......_
 00000670: 5f69 6e69 745f 5fda 0570 726f 7073 da03  _init__..props..
 00000680: 6765 7472 0900 0000 da0c 7061 796c 6f61  getr......payloa
 00000690: 645f 7465 7874 da05 7370 6c69 74da 0463  d_text..split..c
-000006a0: 6270 69da 0973 6174 656c 6c69 7465 da08  bpi..satellite..
-000006b0: 7375 6263 7269 6265 da0a 6f6e 5f6d 6573  subcribe..on_mes
-000006c0: 7361 6765 da09 6d71 7474 5f74 6173 6bda  sage..mqtt_task.
-000006d0: 0576 616c 7565 da03 696e 74da 0774 696d  .value..int..tim
-000006e0: 656f 7574 da04 7469 6d65 da09 7374 6172  eout..time..star
-000006f0: 7474 696d 65da 106e 6f74 6966 6963 6174  ttime..notificat
-00000700: 696f 6e73 656e 64da 0d6e 6578 7463 6865  ionsend..nextche
-00000710: 636b 7469 6d65 da08 6c61 7374 6461 7461  cktime..lastdata
-00000720: da07 6c61 7374 6c6f 67da 0a67 6574 5f73  ..lastlog..get_s
-00000730: 656e 736f 72da 0269 64da 0673 656e 736f  ensor..id..senso
-00000740: 72da 1072 6564 7563 6564 6672 6571 7565  r..reducedfreque
-00000750: 6e63 79da 086b 6574 746c 6569 64da 0b66  ncy..kettleid..f
-00000760: 6572 6d65 6e74 6572 6964 da0e 7265 6475  ermenterid..redu
-00000770: 6365 646c 6f67 6769 6e67 da06 6e6f 7469  cedlogging..noti
-00000780: 6679 da03 7374 72da 046e 616d 6572 0300  fy..str..namer..
-00000790: 0000 da07 5741 524e 494e 4772 0200 0000  ....WARNINGr....
-000007a0: da07 436f 6e66 6972 6d29 04da 0473 656c  ..Confirm)...sel
-000007b0: 6672 2300 0000 7232 0000 0072 1f00 0000  fr#...r2...r....
-000007c0: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-000007d0: 5a63 3a5c 7573 6572 735c 616c 6578 616e  Zc:\users\alexan
-000007e0: 6465 725c 646f 776e 6c6f 6164 735c 6372  der\downloads\cr
-000007f0: 6166 7462 6565 7270 6934 5f61 766f 6c6c  aftbeerpi4_avoll
-00000800: 6b6f 7066 5c63 6270 695c 6578 7465 6e73  kopf\cbpi\extens
-00000810: 696f 6e5c 6d71 7474 5f73 656e 736f 725c  ion\mqtt_sensor\
-00000820: 5f5f 696e 6974 5f5f 2e70 7972 1e00 0000  __init__.pyr....
-00000830: 1500 0000 732e 0000 0000 0114 0110 0110  ....s...........
-00000840: 010a 010e 0116 0106 0114 010a 0106 010e  ................
-00000850: 010a 0106 010e 0114 010a 0106 0110 0110  ................
-00000860: 011a 0218 0106 017a 134d 5154 5453 656e  .......z.MQTTSen
-00000870: 736f 722e 5f5f 696e 6974 5f5f 6301 0000  sor.__init__c...
-00000880: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00000890: 00cb 0000 0073 1a00 0000 7400 a000 a100  .....s....t.....
-000008a0: 7c00 6a01 1700 7c00 5f02 6401 7c00 5f03  |.j...|._.d.|._.
-000008b0: 6400 5300 2902 4e46 2904 722b 0000 0072  d.S.).NF).r+...r
-000008c0: 2a00 0000 722e 0000 0072 2d00 0000 2902  *...r....r-...).
-000008d0: 723d 0000 00da 066b 7761 7267 7372 4000  r=.....kwargsr@.
-000008e0: 0000 7240 0000 0072 4100 0000 723c 0000  ..r@...rA...r<..
-000008f0: 002f 0000 0073 0600 0000 0001 1001 0601  ./...s..........
-00000900: 7a12 4d51 5454 5365 6e73 6f72 2e43 6f6e  z.MQTTSensor.Con
-00000910: 6669 726d 6301 0000 0000 0000 0000 0000  firmc...........
-00000920: 0002 0000 0007 0000 00c3 0000 0073 4a00  .............sJ.
-00000930: 0000 7400 a001 7c00 6a02 a101 7d01 7c00  ..t...|.j...}.|.
-00000940: 6a03 6a04 6401 6402 7405 7c00 6a06 6a07  j.j.d.d.t.|.j.j.
-00000950: 8301 1700 6403 1700 7c01 a008 6404 a101  ....d...|...d...
-00000960: 1700 7409 6a0a 740b 6405 7c00 6a0c 8302  ..t.j.t.d.|.j...
-00000970: 6701 6406 8d04 0100 6400 5300 2907 4e7a  g.d.....d.S.).Nz
-00000980: 124d 5154 5453 656e 736f 7220 5469 6d65  .MQTTSensor Time
-00000990: 6f75 7472 1900 0000 7a27 2720 6469 6420  outr....z'' did 
-000009a0: 6e6f 7420 7265 7370 6f6e 642e 204c 6173  not respond. Las
-000009b0: 7420 6461 7461 2072 6563 6569 7665 643a  t data received:
-000009c0: 207a 0825 4420 2548 3a25 4d72 1a00 0000   z.%D %H:%Mr....
-000009d0: 721b 0000 0029 0d72 0800 0000 da0d 6672  r....).r......fr
-000009e0: 6f6d 7469 6d65 7374 616d 7072 2f00 0000  omtimestampr/...
-000009f0: 7223 0000 0072 3800 0000 7239 0000 0072  r#...r8...r9...r
-00000a00: 3300 0000 723a 0000 00da 0873 7472 6674  3...r:.....strft
-00000a10: 696d 6572 0300 0000 723b 0000 0072 0200  imer....r;...r..
-00000a20: 0000 723c 0000 0029 0272 3d00 0000 da11  ..r<...).r=.....
-00000a30: 7461 7267 6574 5f74 696d 6573 7472 696e  target_timestrin
-00000a40: 6772 4000 0000 7240 0000 0072 4100 0000  gr@...r@...rA...
-00000a50: da07 6d65 7373 6167 6534 0000 0073 0600  ..message4...s..
-00000a60: 0000 0001 0c01 3a01 7a12 4d51 5454 5365  ......:.z.MQTTSe
-00000a70: 6e73 6f72 2e6d 6573 7361 6765 6302 0000  nsor.messagec...
-00000a80: 0000 0000 0000 0000 0005 0000 000a 0000  ................
-00000a90: 00c3 0000 0073 fe00 0000 7400 a001 7c01  .....s....t...|.
-00000aa0: a101 7d02 7aba 7c00 6a02 6400 7501 722e  ..}.z.|.j.d.u.r.
-00000ab0: 7c00 6a02 4400 5d10 7d03 7c02 a003 7c03  |.j.D.].}.|...|.
-00000ac0: 6400 a102 7d02 711c 7404 7c02 7405 7406  d...}.q.t.|.t.t.
-00000ad0: 7407 6603 8302 72c2 7406 7c02 8301 7c00  t.f...r.t.|...|.
-00000ae0: 5f08 7c00 a009 7c00 6a08 a101 0100 7c00  _.|...|.j.....|.
-00000af0: 6a0a 6401 6b02 726e 7c00 a00b a100 4900  j.d.k.rn|.....I.
-00000b00: 6400 4800 0100 6e2a 740c a00d 6402 a00e  d.H...n*t...d...
-00000b10: 7c00 6a0f 6a10 a101 a101 0100 7c00 a011  |.j.j.......|...
-00000b20: 7c00 6a08 a101 0100 7412 a012 a100 7c00  |.j.....t.....|.
-00000b30: 5f13 7c00 6a14 6403 6b03 72c2 7412 a012  _.|.j.d.k.r.t...
-00000b40: a100 7c00 6a14 1700 7c00 5f15 6404 7c00  ..|.j...|._.d.|.
-00000b50: 5f16 7412 a012 a100 7c00 5f17 5700 6e34  _.t.....|._.W.n4
-00000b60: 0400 7418 79f8 0100 7d04 0100 7a1c 740c  ..t.y...}...z.t.
-00000b70: a019 6405 a00e 7c04 a101 a101 0100 5700  ..d...|.......W.
-00000b80: 5900 6400 7d04 7e04 6e0a 6400 7d04 7e04  Y.d.}.~.n.d.}.~.
-00000b90: 3000 3000 6400 5300 2906 4e54 7a1d 4d51  0.0.d.S.).NTz.MQ
-00000ba0: 5454 5365 6e73 6f72 207b 7d20 7265 6775  TTSensor {} regu
-00000bb0: 6c61 7220 6c6f 6767 696e 6772 0100 0000  lar loggingr....
-00000bc0: 467a 144d 5154 5420 5365 6e73 6f72 2045  Fz.MQTT Sensor E
-00000bd0: 7272 6f72 207b 7d29 1ada 046a 736f 6eda  rror {})...json.
-00000be0: 056c 6f61 6473 7221 0000 0072 2000 0000  .loadsr!...r ...
-00000bf0: da0a 6973 696e 7374 616e 6365 7229 0000  ..isinstancer)..
-00000c00: 00da 0566 6c6f 6174 7239 0000 0072 2800  ...floatr9...r(.
-00000c10: 0000 da0b 7075 7368 5f75 7064 6174 6572  ....push_updater
-00000c20: 3700 0000 da08 6c6f 6776 616c 7565 da07  7.....logvalue..
-00000c30: 6c6f 6767 696e 67da 0469 6e66 6fda 0666  logging..info..f
-00000c40: 6f72 6d61 7472 3300 0000 723a 0000 00da  ormatr3...r:....
-00000c50: 086c 6f67 5f64 6174 6172 2b00 0000 7230  .log_datar+...r0
-00000c60: 0000 0072 2a00 0000 722e 0000 0072 2d00  ...r*...r....r-.
-00000c70: 0000 722f 0000 00da 0945 7863 6570 7469  ..r/.....Excepti
-00000c80: 6f6e da05 6572 726f 7229 0572 3d00 0000  on..error).r=...
-00000c90: 7246 0000 00da 0376 616c da03 6b65 79da  rF.....val..key.
-00000ca0: 0165 7240 0000 0072 4000 0000 7241 0000  .er@...r@...rA..
-00000cb0: 0072 2600 0000 3900 0000 7326 0000 0000  .r&...9...s&....
-00000cc0: 010a 0102 010a 010a 010e 0210 010a 010c  ................
-00000cd0: 010a 0110 0214 010c 010a 020a 0110 0106  ................
-00000ce0: 010e 010e 017a 154d 5154 5453 656e 736f  .....z.MQTTSenso
-00000cf0: 722e 6f6e 5f6d 6573 7361 6765 6301 0000  r.on_messagec...
-00000d00: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00000d10: 00c3 0000 0073 9c01 0000 7c00 6a00 6400  .....s....|.j.d.
-00000d20: 7501 7216 7c00 a001 7c00 6a00 a101 6e02  u.r.|...|.j...n.
-00000d30: 6400 7c00 5f02 7c00 6a03 6400 7501 7232  d.|._.|.j.d.u.r2
-00000d40: 7c00 a004 7c00 6a03 a101 6e02 6400 7c00  |...|.j...n.d.|.
-00000d50: 5f05 7406 a006 a100 7d01 7c00 6a02 6400  _.t.....}.|.j.d.
-00000d60: 7501 72e8 7a0e 7c00 6a02 6a07 6a08 7d02  u.r.z.|.j.j.j.}.
-00000d70: 5700 6e10 0100 0100 0100 6401 7d02 5900  W.n.......d.}.Y.
-00000d80: 6e02 3000 7c02 729a 7c00 a009 7c00 6a0a  n.0.|.r.|...|.j.
-00000d90: a101 0100 740b a00c 6402 a00d 7c00 6a0e  ....t...d...|.j.
-00000da0: 6a0f a101 a101 0100 7406 a006 a100 7c00  j.......t.....|.
-00000db0: 5f10 6e4e 740b a00c 6403 a00d 7c00 6a0e  _.nNt...d...|.j.
-00000dc0: 6a0f a101 a101 0100 7c00 6a11 6404 6b03  j.......|.j.d.k.
-00000dd0: 72e8 7c01 7c00 6a10 7c00 6a11 1700 6b05  r.|.|.j.|.j...k.
-00000de0: 72e8 7c00 a009 7c00 6a0a a101 0100 7406  r.|...|.j.....t.
-00000df0: a006 a100 7c00 5f10 740b a00c 6405 a101  ....|._.t...d...
-00000e00: 0100 7c00 6a05 6400 7501 9001 7298 7a0e  ..|.j.d.u...r.z.
-00000e10: 7c00 6a05 6a07 6a08 7d03 5700 6e10 0100  |.j.j.j.}.W.n...
-00000e20: 0100 0100 6401 7d03 5900 6e02 3000 7c03  ....d.}.Y.n.0.|.
-00000e30: 9001 7246 7c00 a009 7c00 6a0a a101 0100  ..rF|...|.j.....
-00000e40: 740b a00c 6406 a00d 7c00 6a0e 6a0f a101  t...d...|.j.j...
-00000e50: a101 0100 7406 a006 a100 7c00 5f10 6e52  ....t.....|._.nR
-00000e60: 740b a00c 6407 a00d 7c00 6a0e 6a0f a101  t...d...|.j.j...
-00000e70: a101 0100 7c00 6a11 6404 6b03 9001 7298  ....|.j.d.k...r.
-00000e80: 7c01 7c00 6a10 7c00 6a11 1700 6b05 9001  |.|.j.|.j...k...
-00000e90: 7298 7c00 a009 7c00 6a0a a101 0100 7406  r.|...|.j.....t.
-00000ea0: a006 a100 7c00 5f10 740b a00c 6405 a101  ....|._.t...d...
-00000eb0: 0100 6400 5300 2908 4e46 7a1b 4d51 5454  ..d.S.).NFz.MQTT
-00000ec0: 5365 6e73 6f72 207b 7d20 4b65 7474 6c65  Sensor {} Kettle
-00000ed0: 2041 6374 6976 657a 1d4d 5154 5453 656e   Activez.MQTTSen
-00000ee0: 736f 7220 7b7d 204b 6574 746c 6520 496e  sor {} Kettle In
-00000ef0: 6163 7469 7665 7201 0000 007a 1c4c 6f67  activer....z.Log
-00000f00: 6765 6420 7769 7468 2072 6564 7563 6564  ged with reduced
-00000f10: 2066 7265 7165 6e63 797a 1e4d 5154 5453   freqencyz.MQTTS
-00000f20: 656e 736f 7220 7b7d 2046 6572 6d65 6e74  ensor {} Ferment
-00000f30: 6572 2041 6374 6976 657a 204d 5154 5453  er Activez MQTTS
-00000f40: 656e 736f 7220 7b7d 2046 6572 6d65 6e74  ensor {} Ferment
-00000f50: 6572 2049 6e61 6374 6976 6529 1272 3500  er Inactive).r5.
-00000f60: 0000 da0a 6765 745f 6b65 7474 6c65 da06  ....get_kettle..
-00000f70: 6b65 7474 6c65 7236 0000 00da 0d67 6574  kettler6.....get
-00000f80: 5f66 6572 6d65 6e74 6572 da09 6665 726d  _fermenter..ferm
-00000f90: 656e 7465 7272 2b00 0000 da08 696e 7374  enterr+.....inst
-00000fa0: 616e 6365 da05 7374 6174 6572 5000 0000  ance..staterP...
-00000fb0: 7228 0000 0072 4d00 0000 724e 0000 0072  r(...rM...rN...r
-00000fc0: 4f00 0000 7233 0000 0072 3a00 0000 7230  O...r3...r:...r0
-00000fd0: 0000 0072 3400 0000 2904 723d 0000 00da  ...r4...).r=....
-00000fe0: 036e 6f77 da0c 6b65 7474 6c65 7374 6174  .now..kettlestat
-00000ff0: 7573 da0f 6665 726d 656e 7465 7273 7461  us..fermentersta
-00001000: 7475 7372 4000 0000 7240 0000 0072 4100  tusr@...r@...rA.
-00001010: 0000 724c 0000 0051 0000 0073 4400 0000  ..rL...Q...sD...
-00001020: 0001 1c01 1c01 0801 0a01 0201 0e01 0601  ................
-00001030: 0a01 0401 0c01 1401 0c02 1401 0a01 1001  ................
-00001040: 0c01 0a01 0a03 0c01 0201 0e01 0601 0a01  ................
-00001050: 0601 0c01 1401 0c02 1401 0c01 1201 0c01  ................
-00001060: 0a01 0a01 7a13 4d51 5454 5365 6e73 6f72  ....z.MQTTSensor
-00001070: 2e6c 6f67 7661 6c75 6563 0100 0000 0000  .logvaluec......
-00001080: 0000 0000 0000 0100 0000 0300 0000 c300  ................
-00001090: 0000 7352 0000 007c 006a 0072 4e7c 006a  ..sR...|.j.rN|.j
-000010a0: 0164 016b 0372 3c74 02a0 02a1 007c 006a  .d.k.r<t.....|.j
-000010b0: 036b 0472 3c7c 006a 0464 026b 0272 3c7c  .k.r<|.j.d.k.r<|
-000010c0: 00a0 05a1 0049 0064 0048 0001 0064 037c  .....I.d.H...d.|
-000010d0: 005f 0474 06a0 0764 04a1 0149 0064 0048  ._.t...d...I.d.H
-000010e0: 0001 0071 0064 0053 0029 054e 7201 0000  ...q.d.S.).Nr...
-000010f0: 0046 54e9 0100 0000 2908 da07 7275 6e6e  .FT.....)...runn
-00001100: 696e 6772 2a00 0000 722b 0000 0072 2e00  ingr*...r+...r..
-00001110: 0000 722d 0000 0072 4600 0000 da07 6173  ..r-...rF.....as
-00001120: 796e 6369 6fda 0573 6c65 6570 a901 723d  yncio..sleep..r=
-00001130: 0000 0072 4000 0000 7240 0000 0072 4100  ...r@...r@...rA.
-00001140: 0000 da03 7275 6e79 0000 0073 0c00 0000  ....runy...s....
-00001150: 0001 0601 0a01 1801 0e01 0601 7a0e 4d51  ............z.MQ
-00001160: 5454 5365 6e73 6f72 2e72 756e 6301 0000  TTSensor.runc...
-00001170: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00001180: 0043 0000 0073 0c00 0000 7400 7c00 6a01  .C...s....t.|.j.
-00001190: 6401 8d01 5300 2902 4e29 0172 2800 0000  d...S.).N).r(...
-000011a0: 2902 da04 6469 6374 7228 0000 0072 6300  )...dictr(...rc.
-000011b0: 0000 7240 0000 0072 4000 0000 7241 0000  ..r@...r@...rA..
-000011c0: 00da 0967 6574 5f73 7461 7465 8100 0000  ...get_state....
-000011d0: 7302 0000 0000 017a 144d 5154 5453 656e  s......z.MQTTSen
-000011e0: 736f 722e 6765 745f 7374 6174 6563 0100  sor.get_statec..
-000011f0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-00001200: 0000 c300 0000 7370 0000 0064 017d 017c  ......sp...d.}.|
-00001210: 006a 00a0 01a1 0073 2274 02a0 0364 02a1  .j.....s"t...d..
-00001220: 0101 007c 006a 00a0 04a1 007d 017a 1a74  ...|.j.....}.z.t
-00001230: 02a0 0364 03a1 0101 007c 006a 0049 0064  ...d.....|.j.I.d
-00001240: 0048 0001 0057 006e 1e04 0074 056a 0679  .H...W.n...t.j.y
-00001250: 5a01 0001 0001 0074 02a0 0364 04a1 0101  Z......t...d....
-00001260: 0059 006e 0230 0074 02a0 0364 05a0 077c  .Y.n.0.t...d...|
-00001270: 01a1 01a1 0101 0064 0053 0029 064e 467a  .......d.S.).NFz
-00001280: 1b54 6173 6b20 6e6f 7420 646f 6e65 202d  .Task not done -
-00001290: 3e20 6361 6e63 656c 6c69 6e67 7a1d 5472  > cancellingz.Tr
-000012a0: 7969 6e67 2074 6f20 6361 6c6c 2063 616e  ying to call can
-000012b0: 6365 6c6c 6564 2074 6173 6b7a 1754 6173  celled taskz.Tas
-000012c0: 6b20 6861 7320 6265 656e 2043 616e 6365  k has been Cance
-000012d0: 6c6c 6564 7a12 5461 736b 2063 616e 6365  lledz.Task cance
-000012e0: 6c6c 6564 3a20 7b7d 2908 7227 0000 00da  lled: {}).r'....
-000012f0: 0464 6f6e 6572 4d00 0000 724e 0000 00da  .donerM...rN....
-00001300: 0663 616e 6365 6c72 6100 0000 da0e 4361  .cancelra.....Ca
-00001310: 6e63 656c 6c65 6445 7272 6f72 724f 0000  ncelledErrorrO..
-00001320: 0029 0272 3d00 0000 5a0d 7761 735f 6361  .).r=...Z.was_ca
-00001330: 6e63 656c 6c65 6472 4000 0000 7240 0000  ncelledr@...r@..
-00001340: 0072 4100 0000 da07 6f6e 5f73 746f 7084  .rA.....on_stop.
-00001350: 0000 0073 1600 0000 0001 0401 0a01 0a01  ...s............
-00001360: 0a01 0201 0a01 1001 0e01 0a01 0601 7a12  ..............z.
-00001370: 4d51 5454 5365 6e73 6f72 2e6f 6e5f 7374  MQTTSensor.on_st
-00001380: 6f70 290c da08 5f5f 6e61 6d65 5f5f da0a  op)...__name__..
-00001390: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000013a0: 616c 6e61 6d65 5f5f 721e 0000 0072 3c00  alname__r....r<.
-000013b0: 0000 7246 0000 0072 2600 0000 724c 0000  ..rF...r&...rL..
-000013c0: 0072 6400 0000 7266 0000 0072 6a00 0000  .rd...rf...rj...
-000013d0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-000013e0: 4000 0000 7240 0000 0072 3e00 0000 7241  @...r@...r>...rA
-000013f0: 0000 0072 1600 0000 0b00 0000 7310 0000  ...r........s...
-00001400: 0008 0a0c 1a08 0508 0508 1808 2808 0808  ............(...
-00001410: 0372 1600 0000 6301 0000 0000 0000 0000  .r....c.........
-00001420: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
-00001430: 2c00 0000 7400 7c00 6a01 a002 6401 6402  ,...t.|.j...d.d.
-00001440: a102 8301 a003 a100 6403 6b02 7228 7c00  ........d.k.r(|.
-00001450: 6a04 a005 6404 7406 a102 0100 6405 5300  j...d.t.....d.S.
-00001460: 2906 7aa2 0a20 2020 2054 6869 7320 6d65  ).z..    This me
-00001470: 7468 6f64 2069 7320 6361 6c6c 6564 2062  thod is called b
-00001480: 7920 7468 6520 7365 7276 6572 2064 7572  y the server dur
-00001490: 696e 6720 7374 6172 7475 700a 2020 2020  ing startup.    
-000014a0: 4865 7265 2079 6f75 206e 6565 6420 746f  Here you need to
-000014b0: 2072 6567 6973 7465 7220 796f 7572 2070   register your p
-000014c0: 6c75 6769 6e73 2061 7420 7468 6520 7365  lugins at the se
-000014d0: 7276 6572 0a0a 2020 2020 3a70 6172 616d  rver..    :param
-000014e0: 2063 6270 693a 2074 6865 2063 6270 6920   cbpi: the cbpi 
-000014f0: 636f 7265 0a20 2020 203a 7265 7475 726e  core.    :return
-00001500: 3a0a 2020 2020 da04 6d71 7474 46da 0474  :.    ..mqttF..t
-00001510: 7275 6572 1600 0000 4e29 0772 3900 0000  ruer....N).r9...
-00001520: da0d 7374 6174 6963 5f63 6f6e 6669 6772  ..static_configr
-00001530: 2000 0000 da05 6c6f 7765 72da 0670 6c75   .....lower..plu
-00001540: 6769 6eda 0872 6567 6973 7465 7272 1600  gin..registerr..
-00001550: 0000 2901 7223 0000 0072 4000 0000 7240  ..).r#...r@...r@
-00001560: 0000 0072 4100 0000 da05 7365 7475 7091  ...rA.....setup.
-00001570: 0000 0073 0400 0000 0008 1a01 7275 0000  ...s........ru..
-00001580: 0029 1272 6100 0000 da14 6362 7069 2e61  .).ra.....cbpi.a
-00001590: 7069 2e64 6174 6163 6c61 7373 6573 7202  pi.dataclassesr.
-000015a0: 0000 0072 0300 0000 5a08 6362 7069 2e61  ...r....Z.cbpi.a
-000015b0: 7069 7204 0000 0072 0500 0000 7206 0000  pir....r....r...
-000015c0: 0072 4d00 0000 7247 0000 0072 2b00 0000  .rM...rG...r+...
-000015d0: 7208 0000 00da 0454 6578 7472 1000 0000  r......Textr....
-000015e0: 7211 0000 00da 064e 756d 6265 7272 1600  r......Numberr..
-000015f0: 0000 7275 0000 0072 4000 0000 7240 0000  ..ru...r@...r@..
-00001600: 0072 4000 0000 7241 0000 00da 083c 6d6f  .r@...rA.....<mo
-00001610: 6475 6c65 3e02 0000 0073 2800 0000 0801  dule>....s(.....
-00001620: 1001 1401 0801 0801 0801 0801 0c02 1001  ................
-00001630: 0a01 02ff 0402 0c01 0c01 0e01 0a01 02ff  ................
-00001640: 04fa 0408 127e                           .....~
+000006a0: 6270 69da 0973 6174 656c 6c69 7465 da09  bpi..satellite..
+000006b0: 7375 6273 6372 6962 65da 0a6f 6e5f 6d65  subscribe..on_me
+000006c0: 7373 6167 65da 0a73 7562 7363 7269 6265  ssage..subscribe
+000006d0: 64da 0576 616c 7565 da03 696e 74da 0774  d..value..int..t
+000006e0: 696d 656f 7574 da04 7469 6d65 da09 7374  imeout..time..st
+000006f0: 6172 7474 696d 65da 106e 6f74 6966 6963  arttime..notific
+00000700: 6174 696f 6e73 656e 64da 0d6e 6578 7463  ationsend..nextc
+00000710: 6865 636b 7469 6d65 da08 6c61 7374 6461  hecktime..lastda
+00000720: 7461 da07 6c61 7374 6c6f 67da 0a67 6574  ta..lastlog..get
+00000730: 5f73 656e 736f 72da 0269 64da 0673 656e  _sensor..id..sen
+00000740: 736f 72da 1072 6564 7563 6564 6672 6571  sor..reducedfreq
+00000750: 7565 6e63 79da 086b 6574 746c 6569 64da  uency..kettleid.
+00000760: 0b66 6572 6d65 6e74 6572 6964 da0e 7265  .fermenterid..re
+00000770: 6475 6365 646c 6f67 6769 6e67 da06 6e6f  ducedlogging..no
+00000780: 7469 6679 da03 7374 72da 046e 616d 6572  tify..str..namer
+00000790: 0300 0000 da07 5741 524e 494e 4772 0200  ......WARNINGr..
+000007a0: 0000 da07 436f 6e66 6972 6d29 04da 0473  ....Confirm)...s
+000007b0: 656c 6672 2300 0000 7232 0000 0072 1f00  elfr#...r2...r..
+000007c0: 0000 a901 da09 5f5f 636c 6173 735f 5fa9  ......__class__.
+000007d0: 00fa 5a63 3a5c 7573 6572 735c 616c 6578  ..Zc:\users\alex
+000007e0: 616e 6465 725c 646f 776e 6c6f 6164 735c  ander\downloads\
+000007f0: 6372 6166 7462 6565 7270 6934 5f61 766f  craftbeerpi4_avo
+00000800: 6c6c 6b6f 7066 5c63 6270 695c 6578 7465  llkopf\cbpi\exte
+00000810: 6e73 696f 6e5c 6d71 7474 5f73 656e 736f  nsion\mqtt_senso
+00000820: 725c 5f5f 696e 6974 5f5f 2e70 7972 1e00  r\__init__.pyr..
+00000830: 0000 1500 0000 732e 0000 0000 0114 0110  ......s.........
+00000840: 0110 010a 010e 0116 0106 0114 010a 0106  ................
+00000850: 010e 010a 0106 010e 0114 010a 0106 0110  ................
+00000860: 0110 011a 0218 0106 017a 134d 5154 5453  .........z.MQTTS
+00000870: 656e 736f 722e 5f5f 696e 6974 5f5f 6301  ensor.__init__c.
+00000880: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000890: 0000 00cb 0000 0073 1a00 0000 7400 a000  .......s....t...
+000008a0: a100 7c00 6a01 1700 7c00 5f02 6401 7c00  ..|.j...|._.d.|.
+000008b0: 5f03 6400 5300 2902 4e46 2904 722b 0000  _.d.S.).NF).r+..
+000008c0: 0072 2a00 0000 722e 0000 0072 2d00 0000  .r*...r....r-...
+000008d0: 2902 723d 0000 00da 066b 7761 7267 7372  ).r=.....kwargsr
+000008e0: 4000 0000 7240 0000 0072 4100 0000 723c  @...r@...rA...r<
+000008f0: 0000 002f 0000 0073 0600 0000 0001 1001  .../...s........
+00000900: 0601 7a12 4d51 5454 5365 6e73 6f72 2e43  ..z.MQTTSensor.C
+00000910: 6f6e 6669 726d 6301 0000 0000 0000 0000  onfirmc.........
+00000920: 0000 0002 0000 0007 0000 00c3 0000 0073  ...............s
+00000930: 4a00 0000 7400 a001 7c00 6a02 a101 7d01  J...t...|.j...}.
+00000940: 7c00 6a03 6a04 6401 6402 7405 7c00 6a06  |.j.j.d.d.t.|.j.
+00000950: 6a07 8301 1700 6403 1700 7c01 a008 6404  j.....d...|...d.
+00000960: a101 1700 7409 6a0a 740b 6405 7c00 6a0c  ....t.j.t.d.|.j.
+00000970: 8302 6701 6406 8d04 0100 6400 5300 2907  ..g.d.....d.S.).
+00000980: 4e7a 124d 5154 5453 656e 736f 7220 5469  Nz.MQTTSensor Ti
+00000990: 6d65 6f75 7472 1900 0000 7a27 2720 6469  meoutr....z'' di
+000009a0: 6420 6e6f 7420 7265 7370 6f6e 642e 204c  d not respond. L
+000009b0: 6173 7420 6461 7461 2072 6563 6569 7665  ast data receive
+000009c0: 643a 207a 0825 4420 2548 3a25 4d72 1a00  d: z.%D %H:%Mr..
+000009d0: 0000 721b 0000 0029 0d72 0800 0000 da0d  ..r....).r......
+000009e0: 6672 6f6d 7469 6d65 7374 616d 7072 2f00  fromtimestampr/.
+000009f0: 0000 7223 0000 0072 3800 0000 7239 0000  ..r#...r8...r9..
+00000a00: 0072 3300 0000 723a 0000 00da 0873 7472  .r3...r:.....str
+00000a10: 6674 696d 6572 0300 0000 723b 0000 0072  ftimer....r;...r
+00000a20: 0200 0000 723c 0000 0029 0272 3d00 0000  ....r<...).r=...
+00000a30: da11 7461 7267 6574 5f74 696d 6573 7472  ..target_timestr
+00000a40: 696e 6772 4000 0000 7240 0000 0072 4100  ingr@...r@...rA.
+00000a50: 0000 da07 6d65 7373 6167 6534 0000 0073  ....message4...s
+00000a60: 0600 0000 0001 0c01 3a01 7a12 4d51 5454  ........:.z.MQTT
+00000a70: 5365 6e73 6f72 2e6d 6573 7361 6765 6302  Sensor.messagec.
+00000a80: 0000 0000 0000 0000 0000 0005 0000 000a  ................
+00000a90: 0000 00c3 0000 0073 0401 0000 7400 a001  .......s....t...
+00000aa0: 7c01 6a02 a003 a100 a101 7d02 7aba 7c00  |.j.......}.z.|.
+00000ab0: 6a04 6400 7501 7234 7c00 6a04 4400 5d10  j.d.u.r4|.j.D.].
+00000ac0: 7d03 7c02 a005 7c03 6400 a102 7d02 7122  }.|...|.d...}.q"
+00000ad0: 7406 7c02 7407 7408 7409 6603 8302 72c8  t.|.t.t.t.f...r.
+00000ae0: 7408 7c02 8301 7c00 5f0a 7c00 a00b 7c00  t.|...|._.|...|.
+00000af0: 6a0a a101 0100 7c00 6a0c 6401 6b02 7274  j.....|.j.d.k.rt
+00000b00: 7c00 a00d a100 4900 6400 4800 0100 6e2a  |.....I.d.H...n*
+00000b10: 740e a00f 6402 a010 7c00 6a11 6a12 a101  t...d...|.j.j...
+00000b20: a101 0100 7c00 a013 7c00 6a0a a101 0100  ....|...|.j.....
+00000b30: 7414 a014 a100 7c00 5f15 7c00 6a16 6403  t.....|._.|.j.d.
+00000b40: 6b03 72c8 7414 a014 a100 7c00 6a16 1700  k.r.t.....|.j...
+00000b50: 7c00 5f17 6404 7c00 5f18 7414 a014 a100  |._.d.|._.t.....
+00000b60: 7c00 5f19 5700 6e34 0400 741a 79fe 0100  |._.W.n4..t.y...
+00000b70: 7d04 0100 7a1c 740e a01b 6405 a010 7c04  }...z.t...d...|.
+00000b80: a101 a101 0100 5700 5900 6400 7d04 7e04  ......W.Y.d.}.~.
+00000b90: 6e0a 6400 7d04 7e04 3000 3000 6400 5300  n.d.}.~.0.0.d.S.
+00000ba0: 2906 4e54 7a1d 4d51 5454 5365 6e73 6f72  ).NTz.MQTTSensor
+00000bb0: 207b 7d20 7265 6775 6c61 7220 6c6f 6767   {} regular logg
+00000bc0: 696e 6772 0100 0000 467a 144d 5154 5420  ingr....Fz.MQTT 
+00000bd0: 5365 6e73 6f72 2045 7272 6f72 207b 7d29  Sensor Error {})
+00000be0: 1cda 046a 736f 6eda 056c 6f61 6473 da07  ...json..loads..
+00000bf0: 7061 796c 6f61 64da 0664 6563 6f64 6572  payload..decoder
+00000c00: 2100 0000 7220 0000 00da 0a69 7369 6e73  !...r .....isins
+00000c10: 7461 6e63 6572 2900 0000 da05 666c 6f61  tancer).....floa
+00000c20: 7472 3900 0000 7228 0000 00da 0b70 7573  tr9...r(.....pus
+00000c30: 685f 7570 6461 7465 7237 0000 00da 086c  h_updater7.....l
+00000c40: 6f67 7661 6c75 65da 076c 6f67 6769 6e67  ogvalue..logging
+00000c50: da04 696e 666f da06 666f 726d 6174 7233  ..info..formatr3
+00000c60: 0000 0072 3a00 0000 da08 6c6f 675f 6461  ...r:.....log_da
+00000c70: 7461 722b 0000 0072 3000 0000 722a 0000  tar+...r0...r*..
+00000c80: 0072 2e00 0000 722d 0000 0072 2f00 0000  .r....r-...r/...
+00000c90: da09 4578 6365 7074 696f 6eda 0565 7272  ..Exception..err
+00000ca0: 6f72 2905 723d 0000 0072 4600 0000 da03  or).r=...rF.....
+00000cb0: 7661 6cda 036b 6579 da01 6572 4000 0000  val..key..er@...
+00000cc0: 7240 0000 0072 4100 0000 7226 0000 0039  r@...rA...r&...9
+00000cd0: 0000 0073 2600 0000 0001 1001 0201 0a01  ...s&...........
+00000ce0: 0a01 0e02 1001 0a01 0c01 0a01 1002 1401  ................
+00000cf0: 0c01 0a02 0a01 1001 0601 0e01 0e01 7a15  ..............z.
+00000d00: 4d51 5454 5365 6e73 6f72 2e6f 6e5f 6d65  MQTTSensor.on_me
+00000d10: 7373 6167 6563 0100 0000 0000 0000 0000  ssagec..........
+00000d20: 0000 0400 0000 0600 0000 c300 0000 739c  ..............s.
+00000d30: 0100 007c 006a 0064 0075 0172 167c 00a0  ...|.j.d.u.r.|..
+00000d40: 017c 006a 00a1 016e 0264 007c 005f 027c  .|.j...n.d.|._.|
+00000d50: 006a 0364 0075 0172 327c 00a0 047c 006a  .j.d.u.r2|...|.j
+00000d60: 03a1 016e 0264 007c 005f 0574 06a0 06a1  ...n.d.|._.t....
+00000d70: 007d 017c 006a 0264 0075 0172 e87a 0e7c  .}.|.j.d.u.r.z.|
+00000d80: 006a 026a 076a 087d 0257 006e 1001 0001  .j.j.j.}.W.n....
+00000d90: 0001 0064 017d 0259 006e 0230 007c 0272  ...d.}.Y.n.0.|.r
+00000da0: 9a7c 00a0 097c 006a 0aa1 0101 0074 0ba0  .|...|.j.....t..
+00000db0: 0c64 02a0 0d7c 006a 0e6a 0fa1 01a1 0101  .d...|.j.j......
+00000dc0: 0074 06a0 06a1 007c 005f 106e 4e74 0ba0  .t.....|._.nNt..
+00000dd0: 0c64 03a0 0d7c 006a 0e6a 0fa1 01a1 0101  .d...|.j.j......
+00000de0: 007c 006a 1164 046b 0372 e87c 017c 006a  .|.j.d.k.r.|.|.j
+00000df0: 107c 006a 1117 006b 0572 e87c 00a0 097c  .|.j...k.r.|...|
+00000e00: 006a 0aa1 0101 0074 06a0 06a1 007c 005f  .j.....t.....|._
+00000e10: 1074 0ba0 0c64 05a1 0101 007c 006a 0564  .t...d.....|.j.d
+00000e20: 0075 0190 0172 987a 0e7c 006a 056a 076a  .u...r.z.|.j.j.j
+00000e30: 087d 0357 006e 1001 0001 0001 0064 017d  .}.W.n.......d.}
+00000e40: 0359 006e 0230 007c 0390 0172 467c 00a0  .Y.n.0.|...rF|..
+00000e50: 097c 006a 0aa1 0101 0074 0ba0 0c64 06a0  .|.j.....t...d..
+00000e60: 0d7c 006a 0e6a 0fa1 01a1 0101 0074 06a0  .|.j.j.......t..
+00000e70: 06a1 007c 005f 106e 5274 0ba0 0c64 07a0  ...|._.nRt...d..
+00000e80: 0d7c 006a 0e6a 0fa1 01a1 0101 007c 006a  .|.j.j.......|.j
+00000e90: 1164 046b 0390 0172 987c 017c 006a 107c  .d.k...r.|.|.j.|
+00000ea0: 006a 1117 006b 0590 0172 987c 00a0 097c  .j...k...r.|...|
+00000eb0: 006a 0aa1 0101 0074 06a0 06a1 007c 005f  .j.....t.....|._
+00000ec0: 1074 0ba0 0c64 05a1 0101 0064 0053 0029  .t...d.....d.S.)
+00000ed0: 084e 467a 1b4d 5154 5453 656e 736f 7220  .NFz.MQTTSensor 
+00000ee0: 7b7d 204b 6574 746c 6520 4163 7469 7665  {} Kettle Active
+00000ef0: 7a1d 4d51 5454 5365 6e73 6f72 207b 7d20  z.MQTTSensor {} 
+00000f00: 4b65 7474 6c65 2049 6e61 6374 6976 6572  Kettle Inactiver
+00000f10: 0100 0000 7a1c 4c6f 6767 6564 2077 6974  ....z.Logged wit
+00000f20: 6820 7265 6475 6365 6420 6672 6571 656e  h reduced freqen
+00000f30: 6379 7a1e 4d51 5454 5365 6e73 6f72 207b  cyz.MQTTSensor {
+00000f40: 7d20 4665 726d 656e 7465 7220 4163 7469  } Fermenter Acti
+00000f50: 7665 7a20 4d51 5454 5365 6e73 6f72 207b  vez MQTTSensor {
+00000f60: 7d20 4665 726d 656e 7465 7220 496e 6163  } Fermenter Inac
+00000f70: 7469 7665 2912 7235 0000 00da 0a67 6574  tive).r5.....get
+00000f80: 5f6b 6574 746c 65da 066b 6574 746c 6572  _kettle..kettler
+00000f90: 3600 0000 da0d 6765 745f 6665 726d 656e  6.....get_fermen
+00000fa0: 7465 72da 0966 6572 6d65 6e74 6572 722b  ter..fermenterr+
+00000fb0: 0000 00da 0869 6e73 7461 6e63 65da 0573  .....instance..s
+00000fc0: 7461 7465 7252 0000 0072 2800 0000 724f  taterR...r(...rO
+00000fd0: 0000 0072 5000 0000 7251 0000 0072 3300  ...rP...rQ...r3.
+00000fe0: 0000 723a 0000 0072 3000 0000 7234 0000  ..r:...r0...r4..
+00000ff0: 0029 0472 3d00 0000 da03 6e6f 77da 0c6b  .).r=.....now..k
+00001000: 6574 746c 6573 7461 7475 73da 0f66 6572  ettlestatus..fer
+00001010: 6d65 6e74 6572 7374 6174 7573 7240 0000  menterstatusr@..
+00001020: 0072 4000 0000 7241 0000 0072 4e00 0000  .r@...rA...rN...
+00001030: 5100 0000 7344 0000 0000 011c 011c 0108  Q...sD..........
+00001040: 010a 0102 010e 0106 010a 0104 010c 0114  ................
+00001050: 010c 0214 010a 0110 010c 010a 010a 030c  ................
+00001060: 0102 010e 0106 010a 0106 010c 0114 010c  ................
+00001070: 0214 010c 0112 010c 010a 010a 017a 134d  .............z.M
+00001080: 5154 5453 656e 736f 722e 6c6f 6776 616c  QTTSensor.logval
+00001090: 7565 6301 0000 0000 0000 0000 0000 0001  uec.............
+000010a0: 0000 0003 0000 00c3 0000 0073 5200 0000  ...........sR...
+000010b0: 7c00 6a00 724e 7c00 6a01 6401 6b03 723c  |.j.rN|.j.d.k.r<
+000010c0: 7402 a002 a100 7c00 6a03 6b04 723c 7c00  t.....|.j.k.r<|.
+000010d0: 6a04 6402 6b02 723c 7c00 a005 a100 4900  j.d.k.r<|.....I.
+000010e0: 6400 4800 0100 6403 7c00 5f04 7406 a007  d.H...d.|._.t...
+000010f0: 6404 a101 4900 6400 4800 0100 7100 6400  d...I.d.H...q.d.
+00001100: 5300 2905 4e72 0100 0000 4654 e901 0000  S.).Nr....FT....
+00001110: 0029 08da 0772 756e 6e69 6e67 722a 0000  .)...runningr*..
+00001120: 0072 2b00 0000 722e 0000 0072 2d00 0000  .r+...r....r-...
+00001130: 7246 0000 00da 0761 7379 6e63 696f da05  rF.....asyncio..
+00001140: 736c 6565 70a9 0172 3d00 0000 7240 0000  sleep..r=...r@..
+00001150: 0072 4000 0000 7241 0000 00da 0372 756e  .r@...rA.....run
+00001160: 7900 0000 730c 0000 0000 0106 010a 0118  y...s...........
+00001170: 010e 0106 017a 0e4d 5154 5453 656e 736f  .....z.MQTTSenso
+00001180: 722e 7275 6e63 0100 0000 0000 0000 0000  r.runc..........
+00001190: 0000 0100 0000 0300 0000 4300 0000 730c  ..........C...s.
+000011a0: 0000 0074 007c 006a 0164 018d 0153 0029  ...t.|.j.d...S.)
+000011b0: 024e 2901 7228 0000 0029 02da 0464 6963  .N).r(...)...dic
+000011c0: 7472 2800 0000 7265 0000 0072 4000 0000  tr(...re...r@...
+000011d0: 7240 0000 0072 4100 0000 da09 6765 745f  r@...rA.....get_
+000011e0: 7374 6174 6581 0000 0073 0200 0000 0001  state....s......
+000011f0: 7a14 4d51 5454 5365 6e73 6f72 2e67 6574  z.MQTTSensor.get
+00001200: 5f73 7461 7465 6301 0000 0000 0000 0000  _statec.........
+00001210: 0000 0001 0000 0004 0000 00c3 0000 0073  ...............s
+00001220: 1a00 0000 7c00 6a00 6a01 a002 7c00 6a03  ....|.j.j...|.j.
+00001230: 7c00 6a04 a102 7c00 5f05 6400 5300 2901  |.j...|._.d.S.).
+00001240: 4e29 0672 2300 0000 7224 0000 00da 0b75  N).r#...r$.....u
+00001250: 6e73 7562 7363 7269 6265 7209 0000 0072  nsubscriber....r
+00001260: 2600 0000 7227 0000 0072 6500 0000 7240  &...r'...re...r@
+00001270: 0000 0072 4000 0000 7241 0000 00da 076f  ...r@...rA.....o
+00001280: 6e5f 7374 6f70 8400 0000 7302 0000 0000  n_stop....s.....
+00001290: 017a 124d 5154 5453 656e 736f 722e 6f6e  .z.MQTTSensor.on
+000012a0: 5f73 746f 7029 0cda 085f 5f6e 616d 655f  _stop)...__name_
+000012b0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+000012c0: 5f71 7561 6c6e 616d 655f 5f72 1e00 0000  _qualname__r....
+000012d0: 723c 0000 0072 4600 0000 7226 0000 0072  r<...rF...r&...r
+000012e0: 4e00 0000 7266 0000 0072 6800 0000 726a  N...rf...rh...rj
+000012f0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00001300: 5f5f 7240 0000 0072 4000 0000 723e 0000  __r@...r@...r>..
+00001310: 0072 4100 0000 7216 0000 000b 0000 0073  .rA...r........s
+00001320: 1000 0000 080a 0c1a 0805 0805 0818 0828  ...............(
+00001330: 0808 0803 7216 0000 0063 0100 0000 0000  ....r....c......
+00001340: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+00001350: 0000 732c 0000 0074 007c 006a 01a0 0264  ..s,...t.|.j...d
+00001360: 0164 02a1 0283 01a0 03a1 0064 036b 0272  .d.........d.k.r
+00001370: 287c 006a 04a0 0564 0474 06a1 0201 0064  (|.j...d.t.....d
+00001380: 0553 0029 067a a20a 2020 2020 5468 6973  .S.).z..    This
+00001390: 206d 6574 686f 6420 6973 2063 616c 6c65   method is calle
+000013a0: 6420 6279 2074 6865 2073 6572 7665 7220  d by the server 
+000013b0: 6475 7269 6e67 2073 7461 7274 7570 0a20  during startup. 
+000013c0: 2020 2048 6572 6520 796f 7520 6e65 6564     Here you need
+000013d0: 2074 6f20 7265 6769 7374 6572 2079 6f75   to register you
+000013e0: 7220 706c 7567 696e 7320 6174 2074 6865  r plugins at the
+000013f0: 2073 6572 7665 720a 0a20 2020 203a 7061   server..    :pa
+00001400: 7261 6d20 6362 7069 3a20 7468 6520 6362  ram cbpi: the cb
+00001410: 7069 2063 6f72 650a 2020 2020 3a72 6574  pi core.    :ret
+00001420: 7572 6e3a 0a20 2020 20da 046d 7174 7446  urn:.    ..mqttF
+00001430: da04 7472 7565 7216 0000 004e 2907 7239  ..truer....N).r9
+00001440: 0000 00da 0d73 7461 7469 635f 636f 6e66  .....static_conf
+00001450: 6967 7220 0000 00da 056c 6f77 6572 da06  igr .....lower..
+00001460: 706c 7567 696e da08 7265 6769 7374 6572  plugin..register
+00001470: 7216 0000 0029 0172 2300 0000 7240 0000  r....).r#...r@..
+00001480: 0072 4000 0000 7241 0000 00da 0573 6574  .r@...rA.....set
+00001490: 7570 8800 0000 7304 0000 0000 081a 0172  up....s........r
+000014a0: 7500 0000 2912 7263 0000 00da 1463 6270  u...).rc.....cbp
+000014b0: 692e 6170 692e 6461 7461 636c 6173 7365  i.api.dataclasse
+000014c0: 7372 0200 0000 7203 0000 005a 0863 6270  sr....r....Z.cbp
+000014d0: 692e 6170 6972 0400 0000 7205 0000 0072  i.apir....r....r
+000014e0: 0600 0000 724f 0000 0072 4700 0000 722b  ....rO...rG...r+
+000014f0: 0000 0072 0800 0000 da04 5465 7874 7210  ...r......Textr.
+00001500: 0000 0072 1100 0000 da06 4e75 6d62 6572  ...r......Number
+00001510: 7216 0000 0072 7500 0000 7240 0000 0072  r....ru...r@...r
+00001520: 4000 0000 7240 0000 0072 4100 0000 da08  @...r@...rA.....
+00001530: 3c6d 6f64 756c 653e 0200 0000 7328 0000  <module>....s(..
+00001540: 0008 0110 0114 0108 0108 0108 0108 010c  ................
+00001550: 0210 010a 0102 ff04 020c 010c 010e 010a  ................
+00001560: 0102 ff04 fa04 0812 75                   ........u
```

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_util/__init__.py` & `cbpi4-4.4.0/cbpi/extension/mqtt_util/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/mqtt_util/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/onewire/__init__.py` & `cbpi4-4.4.0/cbpi/extension/onewire/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/onewire/__pycache__/__init__.cpython-310.pyc` & `cbpi4-4.4.0/cbpi/extension/onewire/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/onewire/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/onewire/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/onewire/__pycache__/__init__.cpython-37.pyc` & `cbpi4-4.4.0/cbpi/extension/onewire/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/onewire/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/onewire/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/timer/__init__.py` & `cbpi4-4.4.0/cbpi/extension/timer/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/timer/__pycache__/__init__.cpython-311.pyc` & `cbpi4-4.4.0/cbpi/extension/timer/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/extension/timer/__pycache__/__init__.cpython-39.pyc` & `cbpi4-4.4.0/cbpi/extension/timer/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_actor.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_config.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_config.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_dashboard.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_dashboard.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_fermentation.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_fermentation.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_fermenterrecipe.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_fermenterrecipe.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_kettle.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_kettle.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_log.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_log.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_login.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_login.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_notification.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_notification.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_plugin.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_plugin.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_recipe.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_recipe.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_sensor.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_sensor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_step.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_step.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_system.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_system.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/http_endpoints/http_upload.py` & `cbpi4-4.4.0/cbpi/http_endpoints/http_upload.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/job/__init__.py` & `cbpi4-4.4.0/cbpi/job/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/job/_job.py` & `cbpi4-4.4.0/cbpi/job/_job.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/job/_scheduler.py` & `cbpi4-4.4.0/cbpi/job/_scheduler.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/job/aiohttp.py` & `cbpi4-4.4.0/cbpi/job/aiohttp.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/satellite.py` & `cbpi4-4.4.0/cbpi/satellite.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/beer_icon.svg` & `cbpi4-4.4.0/cbpi/static/beer_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/calculator_icon.svg` & `cbpi4-4.4.0/cbpi/static/calculator_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/cbpi_icon.svg` & `cbpi4-4.4.0/cbpi/static/cbpi_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/control_icon.svg` & `cbpi4-4.4.0/cbpi/static/control_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/glass_icon.svg` & `cbpi4-4.4.0/cbpi/static/glass_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/grain.svg` & `cbpi4-4.4.0/cbpi/static/grain.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/hops_icon.svg` & `cbpi4-4.4.0/cbpi/static/hops_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/kettle2_icon.svg` & `cbpi4-4.4.0/cbpi/static/kettle2_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/led.svg` & `cbpi4-4.4.0/cbpi/static/led.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/liquid_icon.svg` & `cbpi4-4.4.0/cbpi/static/liquid_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/paddle_icon.svg` & `cbpi4-4.4.0/cbpi/static/paddle_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/pipe_icon.svg` & `cbpi4-4.4.0/cbpi/static/pipe_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/sensor_icon.svg` & `cbpi4-4.4.0/cbpi/static/sensor_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/splash.png` & `cbpi4-4.4.0/cbpi/static/splash.png`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/svg_icon.svg` & `cbpi4-4.4.0/cbpi/static/svg_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/tank_icon.svg` & `cbpi4-4.4.0/cbpi/static/tank_icon.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/target_temp.svg` & `cbpi4-4.4.0/cbpi/static/target_temp.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/thermomenter.svg` & `cbpi4-4.4.0/cbpi/static/thermomenter.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/static/yeast.svg` & `cbpi4-4.4.0/cbpi/static/yeast.svg`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/utils/encoder.py` & `cbpi4-4.4.0/cbpi/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi/websocket.py` & `cbpi4-4.4.0/cbpi/websocket.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/cbpi4.egg-info/PKG-INFO` & `cbpi4-4.4.0/cbpi4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4
-Version: 4.3.2
+Version: 4.4.0
 Summary: CraftBeerPi4 Brewing Software
 Home-page: http://web.craftbeerpi.com
 Author: Manuel Fritsch / Alexander Vollkopf
 Author-email: manuel@craftbeerpi.com
 License: GPLv3
 Project-URL: Documentation, https://openbrewing.gitbook.io/craftbeerpi4_support/
 Platform: UNKNOWN
```

### Comparing `cbpi4-4.3.2/cbpi4.egg-info/SOURCES.txt` & `cbpi4-4.4.0/cbpi4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/setup.py` & `cbpi4-4.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,39 +35,39 @@
       'cbpi': ['*','*.txt', '*.rst', '*.yaml']},
 
       python_requires='>=3.9',
       long_description=long_description,
 	    long_description_content_type='text/markdown',
       install_requires=[
           "typing-extensions>=4",
-          "aiohttp==3.9.3",
+          "aiohttp==3.9.4",
           "aiohttp-auth==0.1.1",
           "aiohttp-route-decorator==0.1.4",
           "aiohttp-security==0.5.0",
           "aiohttp-session==2.12.0",
           "aiohttp-swagger==1.0.16",
           "async-timeout==4.0.3",
           "aiojobs==1.2.1 ",
           "aiosqlite==0.17.0",
-          "cryptography==41.0.7",
-          "pyopenssl==23.3.0",
+          "cryptography==42.0.5",
+          "pyopenssl==24.1.0",
           "requests==2.31.0",
-          "voluptuous==0.13.1",
+          "voluptuous==0.14.2",
           "pyfiglet==1.0.2",
           'click==8.1.7',
-          'shortuuid==1.0.11',
+          'shortuuid==1.0.13',
           'tabulate==0.9.0',
-          'aiomqtt==1.2.1',
-          'inquirer==3.1.3',
+          'aiomqtt==2.0.1',
+          'inquirer==3.2.4',
           'colorama==0.4.6',
-          'psutil==5.9.6',
+          'psutil==5.9.8',
           'cbpi4gui',
           'importlib_metadata',
-          'numpy==1.24.1',
-          'pandas==1.5.3'] + (
+          'numpy==1.26.4',
+          'pandas==2.2.2'] + (
           ['rpi-lgpio'] if raspberrypi else [] ),
 
         dependency_links=[
         'https://testpypi.python.org/pypi',
         
         ],
       entry_points = {
```

### Comparing `cbpi4-4.3.2/tests/cbpi_config_fixture.py` & `cbpi4-4.4.0/tests/cbpi_config_fixture.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_actor.py` & `cbpi4-4.4.0/tests/test_actor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_config.py` & `cbpi4-4.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_dashboard.py` & `cbpi4-4.4.0/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_gpio.py` & `cbpi4-4.4.0/tests/test_gpio.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_index.py` & `cbpi4-4.4.0/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_kettle.py` & `cbpi4-4.4.0/tests/test_kettle.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_logger.py` & `cbpi4-4.4.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_sensor.py` & `cbpi4-4.4.0/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_step.py` & `cbpi4-4.4.0/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `cbpi4-4.3.2/tests/test_ws.py` & `cbpi4-4.4.0/tests/test_ws.py`

 * *Files identical despite different names*

