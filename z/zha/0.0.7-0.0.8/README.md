# Comparing `tmp/zha-0.0.7.tar.gz` & `tmp/zha-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zha-0.0.7.tar", last modified: Fri Apr  5 00:17:11 2024, max compression
+gzip compressed data, was "zha-0.0.8.tar", last modified: Mon Apr 15 14:21:28 2024, max compression
```

## Comparing `zha-0.0.7.tar` & `zha-0.0.8.tar`

### file list

```diff
@@ -1,119 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.682067 zha-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 00:17:07.000000 zha-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 00:17:11.682067 zha-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 00:17:07.000000 zha-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-05 00:17:07.000000 zha-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:17:11.682067 zha-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 00:17:07.000000 zha-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.670066 zha-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_alarm_control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    24049 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_async_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    50883 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    50974 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_cluster_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    29882 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_debouncer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22569 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_device_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    37917 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    27982 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_fan.py
--rw-r--r--   0 runner    (1001) docker     (127)    20992 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    72176 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    39005 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    29709 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-04-05 00:17:07.000000 zha-0.0.7/tests/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.670066 zha-0.0.7/zha/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 00:17:07.000000 zha-0.0.7/zha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    22078 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    26423 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)    12163 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/alarm_control_panel/
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/alarm_control_panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/alarm_control_panel/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/binary_sensor/
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/binary_sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/binary_sensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/button/
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/button/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/button/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.674066 zha-0.0.7/zha/application/platforms/climate/
--rw-r--r--   0 runner    (1001) docker     (127)    31558 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/climate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/climate/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/cover/
--rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/cover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/cover/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/device_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/fan/
--rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/fan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/fan/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/fan/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/light/
--rw-r--r--   0 runner    (1001) docker     (127)    57303 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/light/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/light/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/light/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/lock/
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/lock/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/number/
--rw-r--r--   0 runner    (1001) docker     (127)    34854 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/number/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/application/platforms/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)    57729 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/sensor/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    27338 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-04-05 00:17:07.000000 zha-0.0.7/zha/application/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)    27960 2024-04-05 00:17:07.000000 zha-0.0.7/zha/async_.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-05 00:17:07.000000 zha-0.0.7/zha/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-05 00:17:07.000000 zha-0.0.7/zha/debounce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-05 00:17:07.000000 zha-0.0.7/zha/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-05 00:17:07.000000 zha-0.0.7/zha/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 00:17:07.000000 zha-0.0.7/zha/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-05 00:17:07.000000 zha-0.0.7/zha/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-05 00:17:07.000000 zha-0.0.7/zha/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.678066 zha-0.0.7/zha/zigbee/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.682067 zha-0.0.7/zha/zigbee/cluster_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)    25212 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/closures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    24605 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/hvac.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/lighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/manufacturerspecific.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/registries.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/cluster_handlers/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (127)    37573 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-04-05 00:17:07.000000 zha-0.0.7/zha/zigbee/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:17:11.682067 zha-0.0.7/zha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 00:17:11.000000 zha-0.0.7/zha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.730320 zha-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 14:21:23.000000 zha-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-15 14:21:28.730320 zha-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 14:21:23.000000 zha-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-15 14:21:23.000000 zha-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:21:28.730320 zha-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 14:21:23.000000 zha-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.718320 zha-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_alarm_control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24049 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50883 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50974 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_cluster_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29882 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_debouncer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26484 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38169 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28022 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_fan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72281 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39005 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29750 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23140 2024-04-15 14:21:23.000000 zha-0.0.8/tests/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.718320 zha-0.0.8/zha/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 14:21:23.000000 zha-0.0.8/zha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.722320 zha-0.0.8/zha/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22172 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26616 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.722320 zha-0.0.8/zha/application/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.722320 zha-0.0.8/zha/application/platforms/alarm_control_panel/
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/alarm_control_panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/alarm_control_panel/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.722320 zha-0.0.8/zha/application/platforms/binary_sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/binary_sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/binary_sensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.722320 zha-0.0.8/zha/application/platforms/button/
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/button/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/button/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.726320 zha-0.0.8/zha/application/platforms/climate/
+-rw-r--r--   0 runner    (1001) docker     (127)    31569 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/climate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/climate/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.726320 zha-0.0.8/zha/application/platforms/cover/
+-rw-r--r--   0 runner    (1001) docker     (127)    18271 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/cover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/cover/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/device_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.726320 zha-0.0.8/zha/application/platforms/fan/
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/fan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/fan/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/fan/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.726320 zha-0.0.8/zha/application/platforms/light/
+-rw-r--r--   0 runner    (1001) docker     (127)    55916 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/light/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/light/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/light/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.726320 zha-0.0.8/zha/application/platforms/lock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/lock/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.726320 zha-0.0.8/zha/application/platforms/number/
+-rw-r--r--   0 runner    (1001) docker     (127)    34854 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/number/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.726320 zha-0.0.8/zha/application/platforms/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    57729 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/sensor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27338 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19496 2024-04-15 14:21:23.000000 zha-0.0.8/zha/application/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27960 2024-04-15 14:21:23.000000 zha-0.0.8/zha/async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-15 14:21:23.000000 zha-0.0.8/zha/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-15 14:21:23.000000 zha-0.0.8/zha/debounce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-15 14:21:23.000000 zha-0.0.8/zha/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-15 14:21:23.000000 zha-0.0.8/zha/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 14:21:23.000000 zha-0.0.8/zha/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-15 14:21:23.000000 zha-0.0.8/zha/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-15 14:21:23.000000 zha-0.0.8/zha/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.726320 zha-0.0.8/zha/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.730320 zha-0.0.8/zha/zigbee/cluster_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)    25212 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/closures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24605 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/manufacturerspecific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/cluster_handlers/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36464 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-04-15 14:21:23.000000 zha-0.0.8/zha/zigbee/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:21:28.730320 zha-0.0.8/zha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-15 14:21:28.000000 zha-0.0.8/zha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-15 14:21:28.000000 zha-0.0.8/zha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:21:28.000000 zha-0.0.8/zha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-15 14:21:28.000000 zha-0.0.8/zha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 14:21:28.000000 zha-0.0.8/zha.egg-info/top_level.txt
```

### Comparing `zha-0.0.7/LICENSE` & `zha-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/PKG-INFO` & `zha-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library implementing ZHA for Home Assistant
 Author-email: "David F. Mulcahey" <david.mulcahey@icloud.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zha
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zha-0.0.7/pyproject.toml` & `zha-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_alarm_control_panel.py` & `zha-0.0.8/tests/test_alarm_control_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     "zigpy.zcl.clusters.security.IasAce.client_command",
     new=AsyncMock(return_value=[sentinel.data, zcl_f.Status.SUCCESS]),
 )
 async def test_alarm_control_panel(
     device_joined: Callable[[ZigpyDevice], Awaitable[Device]],
     zigpy_device: ZigpyDevice,  # pylint: disable=redefined-outer-name
     zha_gateway: Gateway,
+    caplog: pytest.LogCaptureFixture,
 ) -> None:
     """Test zhaws alarm control panel platform."""
     zha_device: Device = await device_joined(zigpy_device)
     cluster: security.IasAce = zigpy_device.endpoints.get(1).ias_ace
     alarm_entity: AlarmControlPanel = zha_device.platform_entities.get(
         "00:0d:6f:00:0a:90:69:e7-1"
     )
@@ -180,14 +181,22 @@
     # disarm from panel with good code
     cluster.listener_event(
         "cluster_command", 1, 0, [security.IasAce.ArmMode.Disarm, "4321", 0]
     )
     await zha_gateway.async_block_till_done()
     assert alarm_entity.state["state"] == AlarmState.DISARMED
 
+    # disarm when already disarmed
+    cluster.listener_event(
+        "cluster_command", 1, 0, [security.IasAce.ArmMode.Disarm, "4321", 0]
+    )
+    await zha_gateway.async_block_till_done()
+    assert alarm_entity.state["state"] == AlarmState.DISARMED
+    assert "IAS ACE already disarmed" in caplog.text
+
     # panic from panel
     cluster.listener_event("cluster_command", 1, 4, [])
     await zha_gateway.async_block_till_done()
     assert alarm_entity.state["state"] == AlarmState.TRIGGERED
 
     # reset the panel
     await reset_alarm_panel(zha_gateway, cluster, alarm_entity)
@@ -213,14 +222,20 @@
     await zha_gateway.async_block_till_done()
     assert alarm_entity.state["state"] == AlarmState.TRIGGERED
 
     # reset the panel
     await reset_alarm_panel(zha_gateway, cluster, alarm_entity)
     assert alarm_entity.state["state"] == AlarmState.DISARMED
 
+    alarm_entity._cluster_handler.code_required_arm_actions = True
+    await alarm_entity.async_alarm_arm_away()
+    await zha_gateway.async_block_till_done()
+    assert alarm_entity.state["state"] == AlarmState.DISARMED
+    assert "Invalid code supplied to IAS ACE" in caplog.text
+
 
 async def reset_alarm_panel(
     zha_gateway: Gateway,
     cluster: security.IasAce,
     entity: AlarmControlPanel,
 ) -> None:
     """Reset the state of the alarm panel."""
```

### Comparing `zha-0.0.7/tests/test_async_.py` & `zha-0.0.8/tests/test_async_.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_binary_sensor.py` & `zha-0.0.8/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_button.py` & `zha-0.0.8/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_climate.py` & `zha-0.0.8/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_cluster_handlers.py` & `zha-0.0.8/tests/test_cluster_handlers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_cover.py` & `zha-0.0.8/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_debouncer.py` & `zha-0.0.8/tests/test_debouncer.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_device.py` & `zha-0.0.8/tests/test_device.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,18 +19,21 @@
 from tests.conftest import SIG_EP_INPUT, SIG_EP_OUTPUT, SIG_EP_TYPE
 from zha.application.const import (
     CLUSTER_COMMAND_SERVER,
     CLUSTER_COMMANDS_CLIENT,
     CLUSTER_COMMANDS_SERVER,
     CLUSTER_TYPE_IN,
     CLUSTER_TYPE_OUT,
+    UNKNOWN,
 )
 from zha.application.gateway import Gateway
+from zha.application.platforms.sensor import LQISensor, RSSISensor
+from zha.application.platforms.switch import Switch
 from zha.exceptions import ZHAException
-from zha.zigbee.device import ClusterBinding, Device
+from zha.zigbee.device import ClusterBinding, Device, get_device_automation_triggers
 from zha.zigbee.group import Group
 
 
 @pytest.fixture
 def zigpy_device(
     zigpy_device_mock: Callable[..., ZigpyDevice],
 ) -> Callable[..., ZigpyDevice]:
@@ -395,14 +398,20 @@
     zha_device = await device_joined(zigpy_dev)
 
     assert (
         zha_device.async_get_cluster_attributes(3, general.OnOff.cluster_id)
         == zigpy_dev.endpoints[3].on_off.attributes
     )
 
+    with pytest.raises(KeyError):
+        assert (
+            zha_device.async_get_cluster_attributes(3, general.BinaryValue.cluster_id)
+            is None
+        )
+
 
 async def test_async_get_cluster_commands(
     device_joined: Callable[[ZigpyDevice], Awaitable[Device]],
     zigpy_device: Callable[..., ZigpyDevice],  # pylint: disable=redefined-outer-name
 ) -> None:
     """Test async_get_cluster_commands method."""
     zigpy_dev = zigpy_device(with_basic_cluster_handler=True)
@@ -616,7 +625,97 @@
     await zha_device_remote.async_unbind_from_group(
         group.group_id,
         [ClusterBinding(name="on_off", type=CLUSTER_TYPE_OUT, id=6, endpoint_id=3)],
     )
 
     m1 = "0xb79c: Unbind_req 00:0d:7f:00:0a:90:69:e8, ep: 3, cluster: 6"
     assert f"{m1} to group: 0x1001 completed: [<Status.SUCCESS: 0>]" in caplog.text
+
+
+async def test_device_automation_triggers(
+    device_joined: Callable[[ZigpyDevice], Awaitable[Device]],
+    zigpy_device: Callable[..., ZigpyDevice],  # pylint: disable=redefined-outer-name
+) -> None:
+    """Test device automation triggers."""
+    zigpy_dev = zigpy_device(with_basic_cluster_handler=True)
+    zha_device = await device_joined(zigpy_dev)
+
+    assert get_device_automation_triggers(zha_device) == {
+        ("device_offline", "device_offline"): {"device_event_type": "device_offline"}
+    }
+
+    assert zha_device.device_automation_commands == {}
+    assert zha_device.device_automation_triggers == {
+        ("device_offline", "device_offline"): {"device_event_type": "device_offline"}
+    }
+
+
+async def test_device_properties(
+    device_joined: Callable[[ZigpyDevice], Awaitable[Device]],
+    zigpy_device: Callable[..., ZigpyDevice],  # pylint: disable=redefined-outer-name
+) -> None:
+    """Test device properties."""
+    zigpy_dev = zigpy_device(with_basic_cluster_handler=True)
+    zha_device = await device_joined(zigpy_dev)
+
+    assert zha_device.is_mains_powered is False
+    assert zha_device.is_end_device is True
+    assert zha_device.is_router is False
+    assert zha_device.is_coordinator is False
+    assert zha_device.is_active_coordinator is False
+    assert zha_device.device_type == "EndDevice"
+    assert zha_device.power_source == "Battery or Unknown"
+    assert zha_device.available is True
+    assert zha_device.on_network is True
+    assert zha_device.last_seen is not None
+    assert zha_device.last_seen < time.time()
+
+    assert zha_device.ieee == zigpy_dev.ieee
+    assert zha_device.nwk == zigpy_dev.nwk
+    assert zha_device.manufacturer_code == 0x1037
+    assert zha_device.name == "FakeManufacturer FakeModel"
+    assert zha_device.manufacturer == "FakeManufacturer"
+    assert zha_device.model == "FakeModel"
+    assert zha_device.is_groupable is False
+
+    assert zha_device.power_configuration_ch is None
+    assert zha_device.basic_ch is not None
+    assert zha_device.sw_version is None
+
+    assert len(zha_device.platform_entities) == 3
+    assert "00:0d:6f:00:0a:90:69:e7-3-0-lqi" in zha_device.platform_entities
+    assert "00:0d:6f:00:0a:90:69:e7-3-0-rssi" in zha_device.platform_entities
+    assert "00:0d:6f:00:0a:90:69:e7-3-6" in zha_device.platform_entities
+
+    assert isinstance(
+        zha_device.platform_entities["00:0d:6f:00:0a:90:69:e7-3-0-lqi"], LQISensor
+    )
+    assert isinstance(
+        zha_device.platform_entities["00:0d:6f:00:0a:90:69:e7-3-0-rssi"], RSSISensor
+    )
+    assert isinstance(
+        zha_device.platform_entities["00:0d:6f:00:0a:90:69:e7-3-6"], Switch
+    )
+
+    assert zha_device.get_platform_entity("00:0d:6f:00:0a:90:69:e7-3-0-lqi") is not None
+    assert isinstance(
+        zha_device.get_platform_entity("00:0d:6f:00:0a:90:69:e7-3-0-lqi"), LQISensor
+    )
+
+    with pytest.raises(KeyError, match="Entity foo not found"):
+        zha_device.get_platform_entity("foo")
+
+    # test things are none when they aren't returned by Zigpy
+    zigpy_dev.node_desc = None
+    delattr(zha_device, "manufacturer_code")
+    delattr(zha_device, "is_mains_powered")
+    delattr(zha_device, "device_type")
+    delattr(zha_device, "is_router")
+    delattr(zha_device, "is_end_device")
+    delattr(zha_device, "is_coordinator")
+
+    assert zha_device.manufacturer_code is None
+    assert zha_device.is_mains_powered is None
+    assert zha_device.device_type is UNKNOWN
+    assert zha_device.is_router is None
+    assert zha_device.is_end_device is None
+    assert zha_device.is_coordinator is None
```

### Comparing `zha-0.0.7/tests/test_device_tracker.py` & `zha-0.0.8/tests/test_device_tracker.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_discover.py` & `zha-0.0.8/tests/test_discover.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 import zigpy.zcl.clusters.general
 import zigpy.zcl.clusters.security
 import zigpy.zcl.foundation as zcl_f
 
 from zha.application import Platform, discovery
 from zha.application.discovery import ENDPOINT_PROBE, PLATFORMS, EndpointProbe
 from zha.application.gateway import Gateway
+from zha.application.helpers import DeviceOverridesConfiguration
 from zha.application.platforms import PlatformEntity
 from zha.application.registries import (
     PLATFORM_ENTITIES,
     SINGLE_INPUT_CLUSTER_DEVICE_CLASS,
 )
 from zha.zigbee.cluster_handlers import ClusterHandler
 from zha.zigbee.device import Device
@@ -187,17 +188,15 @@
 
     unhandled_entities = set(created_entities.keys())
 
     for (platform, unique_id), ent_info in device[DEV_SIG_ENT_MAP].items():
         no_tail_id = NO_TAIL_ID.sub("", ent_info[DEV_SIG_ENT_MAP_ID])
         message1 = f"No entity found for platform[{platform}] unique_id[{unique_id}] no_tail_id[{no_tail_id}]"
 
-        if not contains_ignored_suffix(
-            unique_id
-        ):  # TODO remove this when update is fixed
+        if not contains_ignored_suffix(unique_id):
             assert unique_id in created_entities, message1
             entity = created_entities[unique_id]
             unhandled_entities.remove(unique_id)
 
             assert platform == entity.PLATFORM
             assert type(entity).__name__ == ent_info[DEV_SIG_ENT_MAP_CLASS]
             # unique_id used for discover is the same for "multi entities"
@@ -271,15 +270,15 @@
 
     endpoint = mock.MagicMock(spec_set=Endpoint)
     ep_mock = mock.PropertyMock()
     ep_mock.return_value.profile_id = 0x0104
     ep_mock.return_value.device_type = 0x0100
     type(endpoint).zigpy_endpoint = ep_mock
 
-    overrides = {endpoint.unique_id: {"type": Platform.SWITCH}}
+    overrides = {endpoint.unique_id: DeviceOverridesConfiguration(type=Platform.SWITCH)}
     get_entity_mock = mock.MagicMock(
         return_value=(mock.sentinel.entity_cls, mock.sentinel.claimed)
     )
     with (
         mock.patch(
             "zha.application.registries.PLATFORM_ENTITIES.get_entity",
             get_entity_mock,
@@ -324,16 +323,16 @@
     assert endpoint.async_new_entity.call_args[0][1] == mock.sentinel.entity_cls
     assert endpoint.async_new_entity.call_args[0][3] == mock.sentinel.claimed
 
 
 @pytest.mark.parametrize("device_info", DEVICES)
 async def test_discover_endpoint(
     device_info: dict[str, Any],
-    zha_device_mock: Callable[..., Device],
-    zha_gateway: Gateway,
+    zha_device_mock: Callable[..., Device],  # pylint: disable=redefined-outer-name
+    zha_gateway: Gateway,  # pylint: disable=unused-argument
 ) -> None:
     """Test device discovery."""
 
     with mock.patch("zha.zigbee.endpoint.Endpoint.async_new_entity") as new_ent:
         device = await zha_device_mock(
             device_info[SIG_ENDPOINTS],
             manufacturer=device_info[SIG_MANUFACTURER],
@@ -363,28 +362,25 @@
             )
 
     for platform_id, ent_info in device_info[DEV_SIG_ENT_MAP].items():
         platform, unique_id = platform_id
 
         test_ent_class = ent_info[DEV_SIG_ENT_MAP_CLASS]
         test_unique_id_head = UNIQUE_ID_HD.match(unique_id).group(0)
-        if (
-            test_ent_class != "FirmwareUpdateEntity"
-        ):  # TODO remove this when update is fixed
-            assert (test_unique_id_head, test_ent_class) in ha_ent_info
-
-            entity_platform, entity_unique_id, entity_cluster_handlers = ha_ent_info[
-                (test_unique_id_head, test_ent_class)
-            ]
-            assert platform is entity_platform.value
-            # unique_id used for discover is the same for "multi entities"
-            assert unique_id.startswith(entity_unique_id)
-            assert {ch.name for ch in entity_cluster_handlers} == set(
-                ent_info[DEV_SIG_CLUSTER_HANDLERS]
-            )
+        assert (test_unique_id_head, test_ent_class) in ha_ent_info
+
+        entity_platform, entity_unique_id, entity_cluster_handlers = ha_ent_info[
+            (test_unique_id_head, test_ent_class)
+        ]
+        assert platform is entity_platform.value
+        # unique_id used for discover is the same for "multi entities"
+        assert unique_id.startswith(entity_unique_id)
+        assert {ch.name for ch in entity_cluster_handlers} == set(
+            ent_info[DEV_SIG_CLUSTER_HANDLERS]
+        )
 
 
 def _ch_mock(cluster):
     """Return mock of a cluster_handler with a cluster."""
     cluster_handler = mock.MagicMock()
     type(cluster_handler).cluster = mock.PropertyMock(
         return_value=cluster(mock.MagicMock())
@@ -406,16 +402,14 @@
     door_ch = _ch_mock(zigpy.zcl.clusters.closures.DoorLock)
     cover_ch = _ch_mock(zigpy.zcl.clusters.closures.WindowCovering)
     multistate_ch = _ch_mock(zigpy.zcl.clusters.general.MultistateInput)
 
     class QuirkedIAS(zigpy.quirks.CustomCluster, zigpy.zcl.clusters.security.IasZone):
         """Quirked IAS Zone cluster."""
 
-        pass
-
     ias_ch = _ch_mock(QuirkedIAS)
 
     class _Analog(zigpy.quirks.CustomCluster, zigpy.zcl.clusters.general.AnalogInput):
         pass
 
     analog_ch = _ch_mock(_Analog)
 
@@ -481,16 +475,18 @@
         "00:11:22:33:44:55:66:77",
         "manufacturer",
         "model",
         patch_cluster=False,
     )
 
     if override is not None:
-        override = {"device_config": {"00:11:22:33:44:55:66:77-1": {"type": override}}}
-        zha_gateway.config.yaml_config = override
+        overrides = {
+            "00:11:22:33:44:55:66:77-1": DeviceOverridesConfiguration(type=override)
+        }
+        zha_gateway.config.config.device_overrides = overrides
         discovery.ENDPOINT_PROBE.initialize(zha_gateway)
 
     await zha_gateway.async_device_initialized(zigpy_device)
     await zha_gateway.async_block_till_done()
     zha_device = zha_gateway.get_device(zigpy_device.ieee)
 
     entity_id = find_entity_id(
@@ -498,15 +494,15 @@
         zha_device,
     )
     assert entity_id is not None
     assert get_entity(zha_device, entity_id) is not None
 
 
 async def test_quirks_v2_entity_discovery(
-    zha_gateway: Gateway,
+    zha_gateway: Gateway,  # pylint: disable=unused-argument
     zigpy_device_mock,
     device_joined,
 ) -> None:
     """Test quirks v2 discovery."""
 
     zigpy_device = zigpy_device_mock(
         {
@@ -562,15 +558,15 @@
         zha_device,
     )
     assert entity_id is not None
     assert get_entity(zha_device, entity_id) is not None
 
 
 async def test_quirks_v2_entity_discovery_e1_curtain(
-    zha_gateway: Gateway,
+    zha_gateway: Gateway,  # pylint: disable=unused-argument
     zigpy_device_mock,
     device_joined,
 ) -> None:
     """Test quirks v2 discovery for e1 curtain motor."""
 
     class AqaraE1HookState(zigpy.types.enum8):
         """Aqara hook state."""
@@ -774,15 +770,15 @@
         zigpy.zcl.clusters.general.OnOff.AttributeDefs.off_wait_time.name: 3,
     }
     update_attribute_cache(zigpy_device.endpoints[1].on_off)
     return zigpy_device
 
 
 async def test_quirks_v2_entity_no_metadata(
-    zha_gateway: Gateway,
+    zha_gateway: Gateway,  # pylint: disable=unused-argument
     zigpy_device_mock,
     device_joined,
     caplog: pytest.LogCaptureFixture,
 ) -> None:
     """Test quirks v2 discovery skipped - no metadata."""
 
     zigpy_device = _get_test_device(
@@ -793,15 +789,15 @@
     assert (
         f"Device: {str(zigpy_device.ieee)}-{zha_device.name} does not expose any quirks v2 entities"
         in caplog.text
     )
 
 
 async def test_quirks_v2_entity_discovery_errors(
-    zha_gateway: Gateway,
+    zha_gateway: Gateway,  # pylint: disable=unused-argument
     zigpy_device_mock,
     device_joined,
     caplog: pytest.LogCaptureFixture,
 ) -> None:
     """Test quirks v2 discovery skipped - errors."""
 
     zigpy_device = _get_test_device(
@@ -842,15 +838,15 @@
 DEVICE_CLASS_TYPES = [NumberMetadata, BinarySensorMetadata, ZCLSensorMetadata]
 
 
 def validate_device_class_unit(
     quirk: QuirksV2RegistryEntry,
     entity_metadata: EntityMetadata,
     platform: Platform,
-    translations: dict,
+    translations: dict,  # pylint: disable=unused-argument
 ) -> None:
     """Ensure device class and unit are used correctly."""
     if (
         hasattr(entity_metadata, "unit")
         and entity_metadata.unit is not None
         and hasattr(entity_metadata, "device_class")
         and entity_metadata.device_class is not None
@@ -883,15 +879,15 @@
         )
 
 
 def validate_translation_keys_device_class(
     quirk: QuirksV2RegistryEntry,
     entity_metadata: EntityMetadata,
     platform: Platform,
-    translations: dict,
+    translations: dict,  # pylint: disable=unused-argument
 ) -> None:
     """Validate translation keys and device class usage."""
     if isinstance(entity_metadata, ZCLCommandButtonMetadata):
         default_translation_key = entity_metadata.command_name
     else:
         default_translation_key = entity_metadata.attribute_name
     translation_key = entity_metadata.translation_key or default_translation_key
@@ -956,15 +952,15 @@
             bad_device_class_translation_key_usage,
             validate_translation_keys_device_class,
             "cannot have both a translation_key and a device_class",
         ),
     ],
 )
 async def test_quirks_v2_metadata_errors(
-    zha_gateway: Gateway,
+    zha_gateway: Gateway,  # pylint: disable=unused-argument
     zigpy_device_mock,
     device_joined,
     augment_method: Callable[[QuirksV2RegistryEntry], QuirksV2RegistryEntry],
     validate_method: Callable,
     expected_exception_string: str,
 ) -> None:
     """Ensure all v2 quirks translation keys exist."""
@@ -1059,15 +1055,15 @@
         (
             bad_number_device_class,
             f"{ERROR_ROOT}: BadDeviceClass.BAD for platform number",
         ),
     ],
 )
 async def test_quirks_v2_metadata_bad_device_classes(
-    zha_gateway: Gateway,
+    zha_gateway: Gateway,  # pylint: disable=unused-argument
     zigpy_device_mock,
     device_joined,
     caplog: pytest.LogCaptureFixture,
     augment_method: Callable[[QuirksV2RegistryEntry], QuirksV2RegistryEntry],
     expected_exception_string: str,
 ) -> None:
     """Test bad quirks v2 device classes."""
```

### Comparing `zha-0.0.7/tests/test_event.py` & `zha-0.0.8/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_executor.py` & `zha-0.0.8/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_fan.py` & `zha-0.0.8/tests/test_fan.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,16 +304,16 @@
     entity_id = async_find_group_entity_id(Platform.FAN, zha_group)
     assert entity_id is not None
 
     entity: GroupEntity = get_group_entity(zha_group, entity_id)  # type: ignore
     assert entity is not None
 
     assert entity.group_id == zha_group.group_id
-
     assert isinstance(entity, GroupEntity)
+    assert entity.name == zha_group.name
 
     group_fan_cluster = zha_group.zigpy_group.endpoint[hvac.Fan.cluster_id]
 
     dev1_fan_cluster = device_fan_1.device.endpoints[1].fan
     dev2_fan_cluster = device_fan_2.device.endpoints[1].fan
 
     # test that the fan group entity was created and is off
```

### Comparing `zha-0.0.7/tests/test_gateway.py` & `zha-0.0.8/tests/test_gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 from zigpy.zcl.clusters import general, lighting
 import zigpy.zdo.types
 from zigpy.zdo.types import LogicalType, NodeDescriptor
 
 from tests.common import async_find_group_entity_id, find_entity_id
 from tests.conftest import SIG_EP_INPUT, SIG_EP_OUTPUT, SIG_EP_PROFILE, SIG_EP_TYPE
 from zha.application import Platform
+from zha.application.const import CONF_USE_THREAD, RadioType
 from zha.application.gateway import (
+    DeviceJoinedDeviceInfo,
+    DeviceJoinedEvent,
     DevicePairingStatus,
     Gateway,
     RawDeviceInitializedDeviceInfo,
     RawDeviceInitializedEvent,
 )
 from zha.application.helpers import ZHAData
 from zha.application.platforms import GroupEntity, PlatformEntity
@@ -217,15 +220,15 @@
     assert isinstance(entity, GroupEntity)
     assert entity is not None
 
     info = entity.info_object
     assert info.class_name == "LightGroup"
     assert info.platform == Platform.LIGHT
     assert info.unique_id == "light_zha_group_0x0002"
-    assert info.name == "Test Group_0x0002"
+    assert info.name == "Test Group"
     assert info.group_id == zha_group.group_id
     assert info.supported_features == LightEntityFeature.TRANSITION
     assert info.min_mireds == 153
     assert info.max_mireds == 500
     assert info.effect_list is None
 
     device_1_entity_id = find_entity_id(Platform.LIGHT, device_light_1)
@@ -346,24 +349,24 @@
     device_path: str,
     thread_state: bool,
     config_override: dict,
     zigpy_app_controller: ControllerApplication,
     zha_data: ZHAData,
 ) -> None:
     """Test ZHA disabling the UART thread when connecting to a TCP coordinator."""
-    zha_data.config_entry_data["data"]["device"]["path"] = device_path
-    zha_data.yaml_config["zigpy_config"] = config_override
+    zha_data.config.coordinator_configuration.path = device_path
+    zha_data.zigpy_config = config_override
 
     with patch(
         "bellows.zigbee.application.ControllerApplication.new",
         return_value=zigpy_app_controller,
     ) as mock_new:
         zha_gw = Gateway(zha_data)
         await zha_gw.async_initialize()
-        assert mock_new.mock_calls[-1].kwargs["config"]["use_thread"] is thread_state
+        assert mock_new.mock_calls[-1].kwargs["config"][CONF_USE_THREAD] is thread_state
         await zha_gw.shutdown()
 
 
 # pylint: disable=pointless-string-statement
 """TODO
 @pytest.mark.parametrize(
     ("device_path", "config_override", "expected_channel"),
@@ -568,14 +571,36 @@
             ),
             event_type="zha_gateway_message",
             event="raw_device_initialized",
         ),
     )
 
 
+def test_gateway_device_joined(
+    zha_gateway: Gateway,
+    zigpy_dev_basic: ZigpyDevice,  # pylint: disable=redefined-outer-name
+) -> None:
+    """Test Zigpy raw device initialized."""
+
+    zha_gateway.emit = MagicMock(wraps=zha_gateway.emit)
+    zha_gateway.device_joined(zigpy_dev_basic)
+
+    assert zha_gateway.emit.call_count == 1
+    assert zha_gateway.emit.call_args == call(
+        "device_joined",
+        DeviceJoinedEvent(
+            device_info=DeviceJoinedDeviceInfo(
+                ieee=zigpy.types.EUI64.convert("00:0d:6f:00:0a:90:69:e7"),
+                nwk=0xB79C,
+                pairing_status=DevicePairingStatus.PAIRED,
+            )
+        ),
+    )
+
+
 @pytest.mark.looptime
 async def test_pollers_skip(
     zha_gateway: Gateway,
     caplog: pytest.LogCaptureFixture,
 ) -> None:
     """Test pollers skip when they should."""
 
@@ -620,7 +645,33 @@
         1,
         1,
         b"",
     )
 
     assert zha_dev_basic.available is True
     assert zha_dev_basic.on_network is True
+
+
+def test_radio_type():
+    """Test radio type."""
+
+    assert RadioType.list() == [
+        "EZSP = Silicon Labs EmberZNet protocol: Elelabs, HUSBZB-1, Telegesis",
+        "ZNP = Texas Instruments Z-Stack ZNP protocol: CC253x, CC26x2, CC13x2",
+        "deCONZ = dresden elektronik deCONZ protocol: ConBee I/II, RaspBee I/II",
+        "ZiGate = ZiGate Zigbee radios: PiZiGate, ZiGate USB-TTL, ZiGate WiFi",
+        "XBee = Digi XBee Zigbee radios: Digi XBee Series 2, 2C, 3",
+    ]
+
+    assert (
+        RadioType.get_by_description(
+            "EZSP = Silicon Labs EmberZNet protocol: Elelabs, HUSBZB-1, Telegesis"
+        )
+        == RadioType.ezsp
+    )
+
+    assert RadioType.ezsp.description == (
+        "EZSP = Silicon Labs EmberZNet protocol: Elelabs, HUSBZB-1, Telegesis"
+    )
+
+    with pytest.raises(ValueError):
+        RadioType.get_by_description("Invalid description")
```

### Comparing `zha-0.0.7/tests/test_light.py` & `zha-0.0.8/tests/test_light.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,15 @@
 from slugify import slugify
 from zigpy.device import Device as ZigpyDevice
 from zigpy.profiles import zha
 from zigpy.zcl.clusters import general, lighting
 import zigpy.zcl.foundation as zcl_f
 
 from zha.application import Platform
-from zha.application.const import (
-    CONF_ALWAYS_PREFER_XY_COLOR_MODE,
-    CONF_GROUP_MEMBERS_ASSUME_STATE,
-    CUSTOM_CONFIGURATION,
-    ZHA_OPTIONS,
-)
+from zha.application.const import CONF_ALWAYS_PREFER_XY_COLOR_MODE
 from zha.application.gateway import Gateway
 from zha.application.platforms import GroupEntity, PlatformEntity
 from zha.application.platforms.light.const import (
     FLASH_EFFECTS,
     FLASH_LONG,
     FLASH_SHORT,
     ColorMode,
@@ -738,14 +733,15 @@
     assert entity_id is not None
 
     entity: GroupEntity | None = get_group_entity(zha_group, entity_id)
     assert entity is not None
 
     assert isinstance(entity, GroupEntity)
     assert entity.group_id == zha_group.group_id
+    assert entity.name == zha_group.name
 
     device_1_entity_id = find_entity_id(Platform.LIGHT, device_light_1)
     assert device_1_entity_id is not None
     device_2_entity_id = find_entity_id(Platform.LIGHT, device_light_2)
     assert device_2_entity_id is not None
     device_3_entity_id = find_entity_id(Platform.LIGHT, device_light_3)
     assert device_3_entity_id is not None
@@ -1010,18 +1006,17 @@
 
     # create zigpy devices
     zigpy_device = zigpy_device_mock(LIGHT_COLOR)
 
     # mock attribute reads
     zigpy_device.endpoints[1].light_color.PLUGGED_ATTR_READS = plugged_attr_reads
 
+    light_options = zha_gateway.config.config.light_options
     for key in config_override:
-        zha_gateway.config.config_entry_data["options"][CUSTOM_CONFIGURATION][
-            ZHA_OPTIONS
-        ][key] = config_override[key]
+        setattr(light_options, key, config_override[key])
     zha_device = await device_joined(zigpy_device)
     entity_id = find_entity_id(Platform.LIGHT, zha_device)
     assert entity_id is not None
 
     # TODO ensure hue and saturation are properly set on startup
 
 
@@ -1776,14 +1771,21 @@
         manufacturer=None,
         tsn=None,
     )
 
     assert bool(entity.state["on"]) is True
     assert entity.state["color_temp"] == 235
     assert entity.state["color_mode"] == ColorMode.COLOR_TEMP
+    assert entity.supported_color_modes == {ColorMode.COLOR_TEMP, ColorMode.XY}
+    assert entity._supported_color_modes == {
+        ColorMode.COLOR_TEMP,
+        ColorMode.XY,
+        ColorMode.ONOFF,
+        ColorMode.BRIGHTNESS,
+    }
 
     # now let's turn off the Execute_if_off option and see if the old behavior is restored
     dev1_cluster_color.PLUGGED_ATTR_READS = {"options": 0}
     update_attribute_cache(dev1_cluster_color)
 
     # turn off via UI, so the old "enhanced turn on from an off-state" behavior can do something
     await async_test_off_from_client(zha_gateway, dev1_cluster_on_off, entity)
@@ -1853,17 +1855,15 @@
     zha_gateway: Gateway,
     coordinator,  # pylint: disable=redefined-outer-name
     device_light_1,  # pylint: disable=redefined-outer-name
     device_light_2,  # pylint: disable=redefined-outer-name
 ) -> None:
     """Test the group members assume state function."""
 
-    zha_gateway.config.config_entry_data["options"][CUSTOM_CONFIGURATION][ZHA_OPTIONS][
-        CONF_GROUP_MEMBERS_ASSUME_STATE
-    ] = True
+    zha_gateway.config.config.light_options.group_members_assume_state = True
 
     zha_gateway.coordinator_zha_device = coordinator
     coordinator._zha_gateway = zha_gateway
     device_light_1._zha_gateway = zha_gateway
     device_light_2._zha_gateway = zha_gateway
 
     member_ieee_addresses = [device_light_1.ieee, device_light_2.ieee]
```

### Comparing `zha-0.0.7/tests/test_lock.py` & `zha-0.0.8/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_number.py` & `zha-0.0.8/tests/test_number.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Test zha analog output."""
+"""Test zha number platform."""
 
 from collections.abc import Awaitable, Callable
 from unittest.mock import call
 
 import pytest
 from slugify import slugify
 from zigpy.device import Device as ZigpyDevice
@@ -10,14 +10,15 @@
 from zigpy.profiles import zha
 import zigpy.types
 from zigpy.zcl.clusters import general, lighting
 
 from zha.application import Platform
 from zha.application.gateway import Gateway
 from zha.application.platforms import EntityCategory, PlatformEntity
+from zha.application.platforms.number.const import NumberMode
 from zha.exceptions import ZHAException
 from zha.zigbee.device import Device
 
 from .common import (
     find_entity,
     find_entity_id,
     send_attributes_report,
@@ -113,14 +114,21 @@
     assert entity.state["state"] == 15.0
 
     # test attributes
     assert entity.info_object.min_value == 1.0
     assert entity.info_object.max_value == 100.0
     assert entity.info_object.step == 1.1
 
+    assert entity.icon == "mdi:percent"
+    assert entity.native_unit_of_measurement == "%"
+    assert entity.mode == NumberMode.AUTO
+    assert entity.native_min_value == 1.0
+    assert entity.native_max_value == 100.0
+    assert entity.native_step == 1.1
+
     # change value from device
     assert cluster.read_attributes.call_count == 3
     await send_attributes_report(zha_gateway, cluster, {0x0055: 15})
     await zha_gateway.async_block_till_done()
     assert entity.state["state"] == 15.0
 
     # update value from device
@@ -146,42 +154,51 @@
     await zha_gateway.async_block_till_done()
     assert cluster.read_attributes.await_count == 1
     assert cluster.read_attributes.await_args == call(
         ["present_value"], allow_cache=False, only_cache=False, manufacturer=None
     )
     assert entity.state["state"] == 20.0
 
+    await entity.async_set_native_value(30)
+    await zha_gateway.async_block_till_done()
+    assert len(cluster.write_attributes.mock_calls) == 2
+    assert cluster.write_attributes.call_args == call(
+        {"present_value": 30}, manufacturer=None
+    )
+    assert entity.state["state"] == 30.0
+
 
 def get_entity(zha_dev: Device, entity_id: str) -> PlatformEntity:
     """Get entity."""
     entities = {
         entity.PLATFORM + "." + slugify(entity.name, separator="_"): entity
         for entity in zha_dev.platform_entities.values()
     }
     return entities[entity_id]
 
 
 @pytest.mark.parametrize(
-    ("attr", "initial_value", "new_value"),
+    ("attr", "initial_value", "new_value", "max_value"),
     (
-        ("on_off_transition_time", 20, 5),
-        ("on_level", 255, 50),
-        ("on_transition_time", 5, 1),
-        ("off_transition_time", 5, 1),
-        ("default_move_rate", 1, 5),
-        ("start_up_current_level", 254, 125),
+        ("on_off_transition_time", 20, 5, 65535),
+        ("on_level", 255, 50, 255),
+        ("on_transition_time", 5, 1, 65534),
+        ("off_transition_time", 5, 1, 65534),
+        ("default_move_rate", 1, 5, 254),
+        ("start_up_current_level", 254, 125, 255),
     ),
 )
 async def test_level_control_number(
     zha_gateway: Gateway,  # pylint: disable=unused-argument
     light: Device,  # pylint: disable=redefined-outer-name
     device_joined,
     attr: str,
     initial_value: int,
     new_value: int,
+    max_value: int,
 ) -> None:
     """Test ZHA level control number entities - new join."""
 
     level_control_cluster = light.endpoints[1].level
     level_control_cluster.PLUGGED_ATTR_READS = {
         attr: initial_value,
     }
@@ -224,14 +241,21 @@
     ]
 
     entity = get_entity(zha_device, entity_id)
     assert entity
     assert entity.state["state"] == initial_value
     assert entity._attr_entity_category == EntityCategory.CONFIG
 
+    assert entity.icon is None
+    assert entity.native_unit_of_measurement is None
+    assert entity.mode == NumberMode.AUTO
+    assert entity.native_min_value == 0
+    assert entity.native_max_value == max_value
+    assert entity.native_step == 1.0
+
     await entity.async_set_native_value(new_value)
     assert level_control_cluster.write_attributes.mock_calls == [
         call({attr: new_value}, manufacturer=None)
     ]
 
     assert entity.state["state"] == new_value
 
@@ -276,14 +300,23 @@
             allow_cache=False,
             only_cache=False,
             manufacturer=None,
         ),
     ]
     assert entity.state["state"] == new_value
 
+    # update value from device
+    await send_attributes_report(
+        zha_gateway,
+        level_control_cluster,
+        {level_control_cluster.attributes_by_name[attr].id: initial_value},
+    )
+    await zha_gateway.async_block_till_done()
+    assert entity.state["state"] == initial_value
+
 
 @pytest.mark.parametrize(
     ("attr", "initial_value", "new_value"),
     (("start_up_color_temperature", 500, 350),),
 )
 async def test_color_number(
     zha_gateway: Gateway,  # pylint: disable=unused-argument
@@ -381,7 +414,16 @@
             ],
             allow_cache=False,
             only_cache=False,
             manufacturer=None,
         ),
     ]
     assert entity.state["state"] == new_value
+
+    # update value from device
+    await send_attributes_report(
+        zha_gateway,
+        color_cluster,
+        {color_cluster.attributes_by_name[attr].id: initial_value},
+    )
+    await zha_gateway.async_block_till_done()
+    assert entity.state["state"] == initial_value
```

### Comparing `zha-0.0.7/tests/test_registries.py` & `zha-0.0.8/tests/test_registries.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_select.py` & `zha-0.0.8/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_sensor.py` & `zha-0.0.8/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_siren.py` & `zha-0.0.8/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_switch.py` & `zha-0.0.8/tests/test_switch.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,14 +269,15 @@
     assert entity_id is not None
 
     entity: GroupEntity = get_group_entity(zha_group, entity_id)  # type: ignore
     assert entity is not None
 
     assert isinstance(entity, GroupEntity)
     assert entity.group_id == zha_group.group_id
+    assert entity.name == zha_group.name
 
     group_cluster_on_off = zha_group.zigpy_group.endpoint[general.OnOff.cluster_id]
     dev1_cluster_on_off = device_switch_1.device.endpoints[1].on_off
     dev2_cluster_on_off = device_switch_2.device.endpoints[1].on_off
 
     # test that the lights were created and are off
     assert bool(entity.state["state"]) is False
```

### Comparing `zha-0.0.7/tests/test_thread.py` & `zha-0.0.8/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_units.py` & `zha-0.0.8/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/tests/test_update.py` & `zha-0.0.8/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/__init__.py` & `zha-0.0.8/zha/application/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/discovery.py` & `zha-0.0.8/zha/application/discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Device discovery functions for Zigbee Home Automation."""
 
 from __future__ import annotations
 
 from collections import Counter
 import logging
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, cast
 
 from slugify import slugify
 from zigpy.quirks.v2 import (
     BinarySensorMetadata,
     CustomDeviceV2,
     EntityType,
     NumberMetadata,
@@ -19,14 +19,15 @@
     ZCLSensorMetadata,
 )
 from zigpy.state import State
 from zigpy.zcl import ClusterType
 from zigpy.zcl.clusters.general import Ota
 
 from zha.application import Platform, const as zha_const
+from zha.application.helpers import DeviceOverridesConfiguration
 from zha.application.platforms import (  # noqa: F401 pylint: disable=unused-import
     alarm_control_panel,
     binary_sensor,
     button,
     climate,
     cover,
     device_tracker,
@@ -344,15 +345,15 @@
 
 
 class EndpointProbe:
     """All discovered cluster handlers and entities of an endpoint."""
 
     def __init__(self) -> None:
         """Initialize instance."""
-        self._device_configs: dict[str, Any] = {}
+        self._device_configs: dict[str, DeviceOverridesConfiguration] = {}
 
     def discover_entities(self, endpoint: Endpoint) -> None:
         """Process an endpoint on a zigpy device."""
         _LOGGER.debug(
             "Discovering entities for endpoint: %s-%s",
             str(endpoint.device.ieee),
             endpoint.id,
@@ -364,15 +365,17 @@
         PLATFORM_ENTITIES.clean_up()
 
     def discover_by_device_type(self, endpoint: Endpoint) -> None:
         """Process an endpoint on a zigpy device."""
 
         unique_id = endpoint.unique_id
 
-        platform: str | None = self._device_configs.get(unique_id, {}).get("type")
+        platform: str | None = None
+        if unique_id in self._device_configs:
+            platform = self._device_configs.get(unique_id).type
         if platform is None:
             ep_profile_id = endpoint.zigpy_endpoint.profile_id
             ep_device_type = endpoint.zigpy_endpoint.device_type
             platform = DEVICE_CLASS[ep_profile_id].get(ep_device_type)
 
         if platform and platform in PLATFORMS:
             platform = cast(Platform, platform)
@@ -534,16 +537,15 @@
                     entity_and_handler.entity_class,
                     f"{endpoint.unique_id}-{first_ch.cluster.cluster_id}",
                     entity_and_handler.claimed_cluster_handlers,
                 )
 
     def initialize(self, gateway: Gateway) -> None:
         """Update device overrides config."""
-        zha_config = gateway.config.yaml_config
-        if overrides := zha_config.get(zha_const.CONF_DEVICE_CONFIG):
+        if overrides := gateway.config.config.device_overrides:
             self._device_configs.update(overrides)
 
 
 class GroupProbe:
     """Determine the appropriate platform for a group."""
 
     def __init__(self) -> None:
```

### Comparing `zha-0.0.7/zha/application/gateway.py` & `zha-0.0.8/zha/application/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 from functools import cached_property
 import logging
 import time
 from typing import Any, Final, Self, TypeVar, cast
 
 from zhaquirks import setup as setup_quirks
 from zigpy.application import ControllerApplication
-from zigpy.config import CONF_DEVICE, CONF_DEVICE_PATH, CONF_NWK_VALIDATE_SETTINGS
+from zigpy.config import (
+    CONF_DEVICE,
+    CONF_DEVICE_BAUDRATE,
+    CONF_DEVICE_FLOW_CONTROL,
+    CONF_DEVICE_PATH,
+    CONF_NWK_VALIDATE_SETTINGS,
+)
 import zigpy.device
 import zigpy.endpoint
 import zigpy.group
 from zigpy.state import State
 from zigpy.types.named import EUI64
 
 from zha.application import discovery
 from zha.application.const import (
-    CONF_CUSTOM_QUIRKS_PATH,
-    CONF_ENABLE_QUIRKS,
-    CONF_RADIO_TYPE,
     CONF_USE_THREAD,
-    CONF_ZIGPY,
     UNKNOWN_MANUFACTURER,
     UNKNOWN_MODEL,
     ZHA_GW_MSG,
     ZHA_GW_MSG_DEVICE_FULL_INIT,
     ZHA_GW_MSG_DEVICE_JOINED,
     ZHA_GW_MSG_DEVICE_LEFT,
     ZHA_GW_MSG_DEVICE_REMOVED,
@@ -173,17 +175,21 @@
         self._device_availability_checker: DeviceAvailabilityChecker = (
             DeviceAvailabilityChecker(self)
         )
         self.config.gateway = self
 
     def get_application_controller_data(self) -> tuple[ControllerApplication, dict]:
         """Get an uninitialized instance of a zigpy `ControllerApplication`."""
-        radio_type = RadioType[self.config.config_entry_data["data"][CONF_RADIO_TYPE]]
-        app_config = self.config.yaml_config.get(CONF_ZIGPY, {})
-        app_config[CONF_DEVICE] = self.config.config_entry_data["data"][CONF_DEVICE]
+        radio_type = RadioType[self.config.config.coordinator_configuration.radio_type]
+        app_config = self.config.zigpy_config
+        app_config[CONF_DEVICE] = {
+            CONF_DEVICE_PATH: self.config.config.coordinator_configuration.path,
+            CONF_DEVICE_BAUDRATE: self.config.config.coordinator_configuration.baudrate,
+            CONF_DEVICE_FLOW_CONTROL: self.config.config.coordinator_configuration.flow_control,
+        }
 
         if CONF_NWK_VALIDATE_SETTINGS not in app_config:
             app_config[CONF_NWK_VALIDATE_SETTINGS] = True
 
         # The bellows UART thread sometimes propagates a cancellation into the main Core
         # event loop, when a connection to a TCP coordinator fails in a specific way
         if (
@@ -204,17 +210,17 @@
 
     async def async_initialize(self) -> None:
         """Initialize controller and connect radio."""
         discovery.DEVICE_PROBE.initialize(self)
         discovery.ENDPOINT_PROBE.initialize(self)
         discovery.GROUP_PROBE.initialize(self)
 
-        if self.config.yaml_config.get(CONF_ENABLE_QUIRKS, True):
+        if self.config.config.quirks_configuration.enabled:
             await self.async_add_import_executor_job(
-                setup_quirks, self.config.yaml_config.get(CONF_CUSTOM_QUIRKS_PATH)
+                setup_quirks, self.config.config.quirks_configuration.custom_quirks_path
             )
 
         self.shutting_down = False
 
         app_controller_cls, app_config = self.get_application_controller_data()
         app = await app_controller_cls.new(
             config=app_config,
```

### Comparing `zha-0.0.7/zha/application/helpers.py` & `zha-0.0.8/zha/application/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 from zigpy.zcl.foundation import CommandSchema
 import zigpy.zdo.types as zdo_types
 
 from zha.application import Platform
 from zha.application.const import (
     CLUSTER_TYPE_IN,
     CLUSTER_TYPE_OUT,
-    CUSTOM_CONFIGURATION,
+    CONF_DEFAULT_CONSIDER_UNAVAILABLE_BATTERY,
+    CONF_DEFAULT_CONSIDER_UNAVAILABLE_MAINS,
 )
 from zha.async_ import gather_with_limited_concurrency
 from zha.decorators import SetRegistry, callback, periodic
 
 # from zha.zigbee.cluster_handlers.registries import BINDABLE_CLUSTERS
 BINDABLE_CLUSTERS = SetRegistry()
 
@@ -174,26 +175,14 @@
                 source_clusters[endpoint_id][CLUSTER_TYPE_OUT].keys()
             ).intersection(target_clusters[t_endpoint_id][CLUSTER_TYPE_IN].keys())
             if any(bindable in BINDABLE_CLUSTERS for bindable in matches):
                 return True
     return False
 
 
-def async_get_zha_config_value(
-    zha_data: ZHAData, section: str, config_key: str, default: _T
-) -> _T:
-    """Get the value for the specified configuration from the ZHA config entry."""
-    return (
-        zha_data.config_entry_data.get("options", {})
-        .get(CUSTOM_CONFIGURATION, {})
-        .get(section, {})
-        .get(config_key, default)
-    )
-
-
 def convert_install_code(value: str) -> zigpy.types.KeyData:
     """Convert string to install code bytes and validate length."""
 
     try:
         code = binascii.unhexlify(value.replace("-", "").lower())
     except binascii.Error as exc:
         raise vol.Invalid(f"invalid hex string: {value}") from exc
@@ -262,20 +251,98 @@
         # install_code sanity check
         link_key = convert_install_code(install_code)
         return ieee, link_key
 
     raise vol.Invalid(f"couldn't convert qr code: {qr_code}")
 
 
+@dataclass(kw_only=True, slots=True)
+class LightOptions:
+    """ZHA light options."""
+
+    default_light_transition: float = dataclasses.field(default=0)
+    enable_enhanced_light_transition: bool = dataclasses.field(default=False)
+    enable_light_transitioning_flag: bool = dataclasses.field(default=True)
+    always_prefer_xy_color_mode: bool = dataclasses.field(default=True)
+    group_members_assume_state: bool = dataclasses.field(default=True)
+
+
+@dataclass(kw_only=True, slots=True)
+class DeviceOptions:
+    """ZHA device options."""
+
+    enable_identify_on_join: bool = dataclasses.field(default=True)
+    consider_unavailable_mains: int = dataclasses.field(
+        default=CONF_DEFAULT_CONSIDER_UNAVAILABLE_MAINS
+    )
+    consider_unavailable_battery: int = dataclasses.field(
+        default=CONF_DEFAULT_CONSIDER_UNAVAILABLE_BATTERY
+    )
+
+
+@dataclass(kw_only=True, slots=True)
+class AlarmControlPanelOptions:
+    """ZHA alarm control panel options."""
+
+    master_code: str = dataclasses.field(default="1234")
+    failed_tries: int = dataclasses.field(default=3)
+    arm_requires_code: bool = dataclasses.field(default=False)
+
+
+@dataclass(kw_only=True, slots=True)
+class CoordinatorConfiguration:
+    """ZHA coordinator configuration."""
+
+    path: str
+    baudrate: int = dataclasses.field(default=115200)
+    flow_control: str = dataclasses.field(default="hardware")
+    radio_type: str = dataclasses.field(default="ezsp")
+
+
+@dataclass(kw_only=True, slots=True)
+class QuirksConfiguration:
+    """ZHA quirks configuration."""
+
+    enabled: bool = dataclasses.field(default=True)
+    custom_quirks_path: str | None = dataclasses.field(default=None)
+
+
+@dataclass(kw_only=True, slots=True)
+class DeviceOverridesConfiguration:
+    """ZHA device overrides configuration."""
+
+    type: Platform
+
+
+@dataclass(kw_only=True, slots=True)
+class ZHAConfiguration:
+    """ZHA configuration."""
+
+    coordinator_configuration: CoordinatorConfiguration = dataclasses.field(
+        default_factory=CoordinatorConfiguration
+    )
+    quirks_configuration: QuirksConfiguration = dataclasses.field(
+        default_factory=QuirksConfiguration
+    )
+    device_overrides: dict[str, DeviceOverridesConfiguration] = dataclasses.field(
+        default_factory=dict
+    )
+    light_options: LightOptions = dataclasses.field(default_factory=LightOptions)
+    device_options: DeviceOptions = dataclasses.field(default_factory=DeviceOptions)
+    alarm_control_panel_options: AlarmControlPanelOptions = dataclasses.field(
+        default_factory=AlarmControlPanelOptions
+    )
+
+
 @dataclasses.dataclass(kw_only=True, slots=True)
 class ZHAData:
     """ZHA data stored in `gateway.data`."""
 
-    yaml_config: dict[str, Any] = dataclasses.field(default_factory=dict)
-    config_entry_data: dict[str, Any] = dataclasses.field(default_factory=dict)
+    config: ZHAConfiguration
+    zigpy_config: dict[str, Any] = dataclasses.field(default_factory=dict)
     platforms: collections.defaultdict[Platform, list] = dataclasses.field(
         default_factory=lambda: collections.defaultdict(list)
     )
     gateway: Gateway | None = dataclasses.field(default=None)
     device_trigger_cache: dict[str, tuple[str, dict]] = dataclasses.field(
         default_factory=dict
     )
```

### Comparing `zha-0.0.7/zha/application/platforms/__init__.py` & `zha-0.0.8/zha/application/platforms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,15 @@
 
     def __init__(
         self,
         group: Group,
     ) -> None:
         """Initialize a group."""
         super().__init__(f"{self.PLATFORM}_zha_group_0x{group.group_id:04x}")
-        self._name: str = f"{group.name}_0x{group.group_id:04x}"
+        self._attr_name: str = group.name
         self._group: Group = group
         self._group.register_group_entity(self)
 
     @cached_property
     def identifiers(self) -> GroupEntityIdentifiers:
         """Return a dict with the information necessary to identify this entity."""
         return GroupEntityIdentifiers(
@@ -348,22 +348,22 @@
     @cached_property
     def info_object(self) -> GroupEntityInfo:
         """Return a representation of the group."""
         return GroupEntityInfo(
             unique_id=self._unique_id,
             platform=self.PLATFORM,
             class_name=self.__class__.__name__,
-            name=self._name,
+            name=self._attr_name,
             group_id=self.group_id,
         )
 
     @property
     def name(self) -> str:
         """Return the name of the group entity."""
-        return self._name
+        return self._attr_name
 
     @property
     def group_id(self) -> int:
         """Return the group id."""
         return self._group.group_id
 
     @cached_property
```

### Comparing `zha-0.0.7/zha/application/platforms/alarm_control_panel/__init__.py` & `zha-0.0.8/zha/application/platforms/alarm_control_panel/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,14 @@
 import functools
 import logging
 from typing import TYPE_CHECKING, Any
 
 from zigpy.zcl.clusters.security import IasAce
 
 from zha.application import Platform
-from zha.application.const import (
-    CONF_ALARM_ARM_REQUIRES_CODE,
-    CONF_ALARM_FAILED_TRIES,
-    CONF_ALARM_MASTER_CODE,
-    ZHA_ALARM_OPTIONS,
-)
-from zha.application.helpers import async_get_zha_config_value
 from zha.application.platforms import PlatformEntity, PlatformEntityInfo
 from zha.application.platforms.alarm_control_panel.const import (
     IAS_ACE_STATE_MAP,
     SUPPORT_ALARM_ARM_AWAY,
     SUPPORT_ALARM_ARM_HOME,
     SUPPORT_ALARM_ARM_NIGHT,
     SUPPORT_ALARM_TRIGGER,
@@ -72,25 +65,21 @@
         cluster_handlers: list[ClusterHandler],
         endpoint: Endpoint,
         device: Device,
         **kwargs,
     ) -> None:
         """Initialize the ZHA alarm control device."""
         super().__init__(unique_id, cluster_handlers, endpoint, device, **kwargs)
-        config = device.gateway.config
+        alarm_options = device.gateway.config.config.alarm_control_panel_options
         self._cluster_handler: IasAceClusterHandler = cluster_handlers[0]
-        self._cluster_handler.panel_code = async_get_zha_config_value(
-            config, ZHA_ALARM_OPTIONS, CONF_ALARM_MASTER_CODE, "1234"
-        )
-        self._cluster_handler.code_required_arm_actions = async_get_zha_config_value(
-            config, ZHA_ALARM_OPTIONS, CONF_ALARM_ARM_REQUIRES_CODE, False
-        )
-        self._cluster_handler.max_invalid_tries = async_get_zha_config_value(
-            config, ZHA_ALARM_OPTIONS, CONF_ALARM_FAILED_TRIES, 3
+        self._cluster_handler.panel_code = alarm_options.master_code
+        self._cluster_handler.code_required_arm_actions = (
+            alarm_options.arm_requires_code
         )
+        self._cluster_handler.max_invalid_tries = alarm_options.failed_tries
         self._cluster_handler.on_event(
             CLUSTER_HANDLER_STATE_CHANGED, self._handle_event_protocol
         )
 
     @functools.cached_property
     def info_object(self) -> AlarmControlPanelEntityInfo:
         """Return a representation of the alarm control panel."""
```

### Comparing `zha-0.0.7/zha/application/platforms/alarm_control_panel/const.py` & `zha-0.0.8/zha/application/platforms/alarm_control_panel/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/binary_sensor/__init__.py` & `zha-0.0.8/zha/application/platforms/binary_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/binary_sensor/const.py` & `zha-0.0.8/zha/application/platforms/binary_sensor/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/button/__init__.py` & `zha-0.0.8/zha/application/platforms/button/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/climate/__init__.py` & `zha-0.0.8/zha/application/platforms/climate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,30 +92,36 @@
         device: Device,
         **kwargs,
     ):
         """Initialize ZHA Thermostat instance."""
         super().__init__(unique_id, cluster_handlers, endpoint, device, **kwargs)
         self._preset = Preset.NONE
         self._presets = []
-        self._supported_flags = (
-            ClimateEntityFeature.TARGET_TEMPERATURE
-            | ClimateEntityFeature.TURN_OFF
-            | ClimateEntityFeature.TURN_ON
-        )
+
         self._thermostat_cluster_handler: ClusterHandler = self.cluster_handlers.get(
             CLUSTER_HANDLER_THERMOSTAT
         )
         self._fan_cluster_handler: ClusterHandler = self.cluster_handlers.get(
             CLUSTER_HANDLER_FAN
         )
         self._thermostat_cluster_handler.on_event(
             CLUSTER_HANDLER_ATTRIBUTE_UPDATED,
             self.handle_cluster_handler_attribute_updated,
         )
 
+        self._supported_features = (
+            ClimateEntityFeature.TARGET_TEMPERATURE
+            | ClimateEntityFeature.TURN_OFF
+            | ClimateEntityFeature.TURN_ON
+        )
+        if HVACMode.HEAT_COOL in self.hvac_modes:
+            self._supported_features |= ClimateEntityFeature.TARGET_TEMPERATURE_RANGE
+        if self._fan_cluster_handler is not None:
+            self._supported_features |= ClimateEntityFeature.FAN_MODE
+
     @functools.cached_property
     def info_object(self) -> ThermostatEntityInfo:
         """Return a representation of the thermostat."""
         return ThermostatEntityInfo(
             **super().info_object.__dict__,
             max_temp=self.max_temp,
             min_temp=self.min_temp,
@@ -283,20 +289,15 @@
     def preset_modes(self) -> list[str] | None:
         """Return supported preset modes."""
         return self._presets
 
     @functools.cached_property
     def supported_features(self) -> ClimateEntityFeature:
         """Return the list of supported features."""
-        features = self._supported_flags
-        if HVACMode.HEAT_COOL in self.hvac_modes:
-            features |= ClimateEntityFeature.TARGET_TEMPERATURE_RANGE
-        if self._fan_cluster_handler is not None:
-            self._supported_flags |= ClimateEntityFeature.FAN_MODE
-        return features
+        return self._supported_features
 
     @property
     def target_temperature(self):
         """Return the temperature we try to reach."""
         temp = None
         if self.hvac_mode == HVACMode.COOL:
             if self.preset_mode == Preset.AWAY:
@@ -505,15 +506,15 @@
         endpoint: Endpoint,
         device: Device,
         **kwargs,
     ):
         """Initialize ZHA Thermostat instance."""
         super().__init__(unique_id, cluster_handlers, endpoint, device, **kwargs)
         self._presets = [Preset.AWAY, Preset.NONE]
-        self._supported_flags |= ClimateEntityFeature.PRESET_MODE
+        self._supported_features |= ClimateEntityFeature.PRESET_MODE
         self._manufacturer_ch = self.cluster_handlers["sinope_manufacturer_specific"]
 
         self._tracked_tasks.append(
             device.gateway.async_create_background_task(
                 self._update_time(),
                 name=f"sinope_time_updater_{self.unique_id}",
                 eager_start=True,
@@ -628,15 +629,15 @@
             Preset.AWAY,
             Preset.SCHEDULE,
             Preset.COMFORT,
             Preset.ECO,
             Preset.BOOST,
             Preset.COMPLEX,
         ]
-        self._supported_flags |= ClimateEntityFeature.PRESET_MODE
+        self._supported_features |= ClimateEntityFeature.PRESET_MODE
 
     @functools.cached_property
     def hvac_modes(self) -> list[HVACMode]:
         """Return only the heat mode, because the device can't be turned off."""
         return [HVACMode.HEAT]
 
     def handle_cluster_handler_attribute_updated(
@@ -716,15 +717,15 @@
             Preset.NONE,
             Preset.AWAY,
             Preset.SCHEDULE,
             Preset.ECO,
             Preset.BOOST,
             Preset.TEMP_MANUAL,
         ]
-        self._supported_flags |= ClimateEntityFeature.PRESET_MODE
+        self._supported_features |= ClimateEntityFeature.PRESET_MODE
 
     @functools.cached_property
     def hvac_modes(self) -> list[HVACMode]:
         """Return only the heat mode, because the device can't be turned off."""
         return [HVACMode.HEAT]
 
     def handle_cluster_handler_attribute_updated(
@@ -825,15 +826,15 @@
         super().__init__(unique_id, cluster_handlers, endpoint, device, **kwargs)
         self._presets = [
             Preset.NONE,
             self.PRESET_HOLIDAY,
             Preset.SCHEDULE,
             self.PRESET_FROST,
         ]
-        self._supported_flags |= ClimateEntityFeature.PRESET_MODE
+        self._supported_features |= ClimateEntityFeature.PRESET_MODE
 
     def handle_cluster_handler_attribute_updated(
         self, event: ClusterAttributeUpdatedEvent
     ) -> None:
         """Handle attribute update from device."""
         if event.attribute_name == "operation_preset":
             if event.attribute_value == 0:
```

### Comparing `zha-0.0.7/zha/application/platforms/climate/const.py` & `zha-0.0.8/zha/application/platforms/climate/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/cover/__init__.py` & `zha-0.0.8/zha/application/platforms/cover/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/cover/const.py` & `zha-0.0.8/zha/application/platforms/cover/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/device_tracker.py` & `zha-0.0.8/zha/application/platforms/device_tracker.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/fan/__init__.py` & `zha-0.0.8/zha/application/platforms/fan/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/fan/const.py` & `zha-0.0.8/zha/application/platforms/fan/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/fan/helpers.py` & `zha-0.0.8/zha/application/platforms/fan/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/helpers.py` & `zha-0.0.8/zha/application/platforms/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/light/__init__.py` & `zha-0.0.8/zha/application/platforms/light/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,23 +17,14 @@
 
 from zigpy.types import EUI64
 from zigpy.zcl.clusters.general import Identify, LevelControl, OnOff
 from zigpy.zcl.clusters.lighting import Color
 from zigpy.zcl.foundation import Status
 
 from zha.application import Platform
-from zha.application.const import (
-    CONF_ALWAYS_PREFER_XY_COLOR_MODE,
-    CONF_DEFAULT_LIGHT_TRANSITION,
-    CONF_ENABLE_ENHANCED_LIGHT_TRANSITION,
-    CONF_ENABLE_LIGHT_TRANSITIONING_FLAG,
-    CONF_GROUP_MEMBERS_ASSUME_STATE,
-    ZHA_OPTIONS,
-)
-from zha.application.helpers import async_get_zha_config_value
 from zha.application.platforms import (
     BaseEntity,
     BaseEntityInfo,
     GroupEntity,
     PlatformEntity,
 )
 from zha.application.platforms.helpers import (
@@ -140,14 +131,15 @@
         self._state: bool | None
         self._brightness: int | None = None
         self._off_with_transition: bool = False
         self._off_brightness: int | None = None
         self._effect_list: list[str] | None = None
         self._effect: str | None = None
         self._supported_color_modes: set[ColorMode] = set()
+        self._external_supported_color_modes: set[ColorMode] = set()
         self._zha_config_transition: int = self._DEFAULT_MIN_TRANSITION_TIME
         self._zha_config_enhanced_light_transition: bool = False
         self._zha_config_enable_light_transitioning_flag: bool = True
         self._zha_config_always_prefer_xy_color_mode: bool = True
         self._on_off_cluster_handler: ClusterHandler = None
         self._level_cluster_handler: ClusterHandler = None
         self._color_cluster_handler: ClusterHandler = None
@@ -207,15 +199,15 @@
     def supported_features(self) -> int:
         """Flag supported features."""
         return self._supported_features
 
     @property
     def supported_color_modes(self) -> set[ColorMode]:
         """Flag supported color modes."""
-        return self._supported_color_modes
+        return self._external_supported_color_modes
 
     @property
     def is_on(self) -> bool:
         """Return true if entity is on."""
         if self._state is None:
             return False
         return self._state
@@ -248,31 +240,14 @@
                 event,
             )
             return
         value = max(0, min(254, event.level))
         self._brightness = value
         self.maybe_emit_state_changed_event()
 
-    def set_level(self, value: int) -> None:
-        """Set the brightness of this light between 0..254.
-
-        brightness level 255 is a special value instructing the device to come
-        on at `on_level` Zigbee attribute value, regardless of the last set
-        level
-        """
-        if self.is_transitioning:
-            self.debug(
-                "received level %s while transitioning - skipping update",
-                value,
-            )
-            return
-        value = max(0, min(254, value))
-        self._brightness = value
-        self.maybe_emit_state_changed_event()
-
     async def async_turn_on(self, **kwargs: Any) -> None:
         """Turn the entity on."""
         transition = kwargs.get(ATTR_TRANSITION)
         duration = (
             transition if transition is not None else self._zha_config_transition
         ) or (
             # if 0 is passed in some devices still need the minimum default
@@ -706,14 +681,15 @@
     cluster_handler_names=CLUSTER_HANDLER_ON_OFF,
     aux_cluster_handlers={CLUSTER_HANDLER_COLOR, CLUSTER_HANDLER_LEVEL},
 )
 class Light(PlatformEntity, BaseLight):
     """Representation of a ZHA or ZLL light."""
 
     _supported_color_modes: set[ColorMode]
+    _external_supported_color_modes: set[ColorMode]
     _attr_translation_key: str = "light"
     _REFRESH_INTERVAL = (2700, 4500)
     __polling_interval: int
 
     def __init__(
         self,
         unique_id: str,
@@ -737,19 +713,17 @@
         self._identify_cluster_handler: ClusterHandler = device.identify_ch
         if self._color_cluster_handler:
             self._min_mireds: int = self._color_cluster_handler.min_mireds
             self._max_mireds: int = self._color_cluster_handler.max_mireds
         self._cancel_refresh_handle: Callable | None = None
         effect_list = []
 
-        self._zha_config_always_prefer_xy_color_mode = async_get_zha_config_value(
-            device.gateway.config,
-            ZHA_OPTIONS,
-            CONF_ALWAYS_PREFER_XY_COLOR_MODE,
-            True,
+        light_options = device.gateway.config.config.light_options
+        self._zha_config_always_prefer_xy_color_mode = (
+            light_options.always_prefer_xy_color_mode
         )
 
         self._supported_color_modes = {ColorMode.ONOFF}
         if self._level_cluster_handler:
             self._supported_color_modes.add(ColorMode.BRIGHTNESS)
             self._supported_features |= LightEntityFeature.TRANSITION
             self._brightness = self._level_cluster_handler.current_level
@@ -799,16 +773,16 @@
                 )
 
             if self._color_cluster_handler.color_loop_supported:
                 self._supported_features |= LightEntityFeature.EFFECT
                 effect_list.append(EFFECT_COLORLOOP)
                 if self._color_cluster_handler.color_loop_active == 1:
                     self._effect = EFFECT_COLORLOOP
-        supported_color_modes: set[ColorMode] = filter_supported_color_modes(
-            self._supported_color_modes
+        self._external_supported_color_modes = supported_color_modes = (
+            filter_supported_color_modes(self._supported_color_modes)
         )
         if len(supported_color_modes) == 1:
             self._color_mode = next(iter(supported_color_modes))
         else:  # Light supports color_temp + hs, determine which mode the light is in
             assert self._color_cluster_handler
             if (
                 self._color_cluster_handler.color_mode
@@ -820,31 +794,20 @@
 
         if self._identify_cluster_handler:
             self._supported_features |= LightEntityFeature.FLASH
 
         if effect_list:
             self._effect_list = effect_list
 
-        self._zha_config_transition = async_get_zha_config_value(
-            device.gateway.config,
-            ZHA_OPTIONS,
-            CONF_DEFAULT_LIGHT_TRANSITION,
-            0,
-        )
-        self._zha_config_enhanced_light_transition = async_get_zha_config_value(
-            device.gateway.config,
-            ZHA_OPTIONS,
-            CONF_ENABLE_ENHANCED_LIGHT_TRANSITION,
-            False,
-        )
-        self._zha_config_enable_light_transitioning_flag = async_get_zha_config_value(
-            device.gateway.config,
-            ZHA_OPTIONS,
-            CONF_ENABLE_LIGHT_TRANSITIONING_FLAG,
-            True,
+        self._zha_config_transition = light_options.default_light_transition
+        self._zha_config_enhanced_light_transition = (
+            light_options.enable_enhanced_light_transition
+        )
+        self._zha_config_enable_light_transitioning_flag = (
+            light_options.enable_light_transitioning_flag
         )
 
         self._on_off_cluster_handler.on_event(
             CLUSTER_HANDLER_ATTRIBUTE_UPDATED,
             self.handle_cluster_handler_attribute_updated,
         )
 
@@ -1166,37 +1129,24 @@
         self._color_cluster_handler: None | (
             ClusterHandler
         ) = group.zigpy_group.endpoint[Color.cluster_id]
         self._identify_cluster_handler: None | (
             ClusterHandler
         ) = group.zigpy_group.endpoint[Identify.cluster_id]
         self._debounced_member_refresh: Debouncer | None = None
-        self._zha_config_transition = async_get_zha_config_value(
-            group.gateway.config,
-            ZHA_OPTIONS,
-            CONF_DEFAULT_LIGHT_TRANSITION,
-            0,
-        )
-        self._zha_config_enable_light_transitioning_flag = async_get_zha_config_value(
-            group.gateway.config,
-            ZHA_OPTIONS,
-            CONF_ENABLE_LIGHT_TRANSITIONING_FLAG,
-            True,
-        )
-        self._zha_config_always_prefer_xy_color_mode = async_get_zha_config_value(
-            group.gateway.config,
-            ZHA_OPTIONS,
-            CONF_ALWAYS_PREFER_XY_COLOR_MODE,
-            True,
-        )
-        self._zha_config_group_members_assume_state = async_get_zha_config_value(
-            group.gateway.config,
-            ZHA_OPTIONS,
-            CONF_GROUP_MEMBERS_ASSUME_STATE,
-            True,
+        light_options = group.gateway.config.config.light_options
+        self._zha_config_transition = light_options.default_light_transition
+        self._zha_config_enable_light_transitioning_flag = (
+            light_options.enable_light_transitioning_flag
+        )
+        self._zha_config_always_prefer_xy_color_mode = (
+            light_options.always_prefer_xy_color_mode
+        )
+        self._zha_config_group_members_assume_state = (
+            light_options.group_members_assume_state
         )
         if self._zha_config_group_members_assume_state:
             self._update_group_from_child_delay = ASSUME_UPDATE_GROUP_FROM_CHILD_DELAY
         self._zha_config_enhanced_light_transition = False
 
         self._color_mode = ColorMode.UNKNOWN
         self._supported_color_modes = {ColorMode.ONOFF}
@@ -1316,16 +1266,16 @@
         all_supported_color_modes: list[set[ColorMode]] = list(
             find_state_attributes(states, ATTR_SUPPORTED_COLOR_MODES)
         )
         self._supported_color_modes = set().union(*all_supported_color_modes)
 
         if all_supported_color_modes:
             # Merge all color modes.
-            supported_color_modes = filter_supported_color_modes(
-                set().union(*all_supported_color_modes)
+            self._external_supported_color_modes = supported_color_modes = (
+                filter_supported_color_modes(set().union(*all_supported_color_modes))
             )
 
         self._color_mode = ColorMode.UNKNOWN
         all_color_modes = list(find_state_attributes(on_states, ATTR_COLOR_MODE))
         if all_color_modes:
             # Report the most common color mode, select brightness and onoff last
             color_mode_count = Counter(itertools.chain(all_color_modes))
```

### Comparing `zha-0.0.7/zha/application/platforms/light/const.py` & `zha-0.0.8/zha/application/platforms/light/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/lock/__init__.py` & `zha-0.0.8/zha/application/platforms/lock/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/number/__init__.py` & `zha-0.0.8/zha/application/platforms/number/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -238,14 +238,18 @@
     ) -> None:
         """Init this number configuration entity."""
         self._cluster_handler: ClusterHandler = cluster_handlers[0]
         self._attr_device_class: NumberDeviceClass | None = None
         if ENTITY_METADATA in kwargs:
             self._init_from_quirks_metadata(kwargs[ENTITY_METADATA])
         super().__init__(unique_id, cluster_handlers, endpoint, device, **kwargs)
+        self._cluster_handler.on_event(
+            CLUSTER_HANDLER_ATTRIBUTE_UPDATED,
+            self.handle_cluster_handler_attribute_updated,
+        )
 
     def _init_from_quirks_metadata(self, entity_metadata: NumberMetadata) -> None:
         """Init this entity from the quirks metadata."""
         super()._init_from_quirks_metadata(entity_metadata)
         self._attribute_name = entity_metadata.attribute_name
 
         if entity_metadata.min is not None:
@@ -263,18 +267,14 @@
                 Platform.NUMBER.value,
                 _LOGGER,
             )
         if entity_metadata.device_class is None and entity_metadata.unit is not None:
             self._attr_native_unit_of_measurement = validate_unit(
                 entity_metadata.unit
             ).value
-        self._cluster_handler.on_event(
-            CLUSTER_HANDLER_ATTRIBUTE_UPDATED,
-            self.handle_cluster_handler_attribute_updated,
-        )
 
     @functools.cached_property
     def info_object(self) -> NumberConfigurationEntityInfo:
         """Return a representation of the number entity."""
         return NumberConfigurationEntityInfo(
             **super().info_object.__dict__,
             min_value=self._attr_native_min_value,
```

### Comparing `zha-0.0.7/zha/application/platforms/number/const.py` & `zha-0.0.8/zha/application/platforms/number/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/select.py` & `zha-0.0.8/zha/application/platforms/select.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/sensor/__init__.py` & `zha-0.0.8/zha/application/platforms/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/sensor/const.py` & `zha-0.0.8/zha/application/platforms/sensor/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/siren.py` & `zha-0.0.8/zha/application/platforms/siren.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/switch.py` & `zha-0.0.8/zha/application/platforms/switch.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/platforms/update.py` & `zha-0.0.8/zha/application/platforms/update.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/application/registries.py` & `zha-0.0.8/zha/application/registries.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/async_.py` & `zha-0.0.8/zha/async_.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/debounce.py` & `zha-0.0.8/zha/debounce.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/decorators.py` & `zha-0.0.8/zha/decorators.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/event.py` & `zha-0.0.8/zha/event.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/mixins.py` & `zha-0.0.8/zha/mixins.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/units.py` & `zha-0.0.8/zha/units.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/__init__.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/closures.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/closures.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/const.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/const.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/general.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/general.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/helpers.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/helpers.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/homeautomation.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/homeautomation.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/hvac.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/hvac.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/lighting.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/lighting.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/lightlink.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/lightlink.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/manufacturerspecific.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/manufacturerspecific.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/measurement.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/measurement.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/protocol.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/protocol.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/security.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/security.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/cluster_handlers/smartenergy.py` & `zha-0.0.8/zha/zigbee/cluster_handlers/smartenergy.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/device.py` & `zha-0.0.8/zha/zigbee/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Device for Zigbee Home Automation."""
 
 # pylint: disable=too-many-lines
 
 from __future__ import annotations
 
 import asyncio
-from contextlib import suppress
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
 import logging
 import time
 from typing import TYPE_CHECKING, Any, Final, Self
 
@@ -47,30 +46,24 @@
     ATTR_QUIRK_ID,
     ATTR_VALUE,
     CLUSTER_COMMAND_SERVER,
     CLUSTER_COMMANDS_CLIENT,
     CLUSTER_COMMANDS_SERVER,
     CLUSTER_TYPE_IN,
     CLUSTER_TYPE_OUT,
-    CONF_CONSIDER_UNAVAILABLE_BATTERY,
-    CONF_CONSIDER_UNAVAILABLE_MAINS,
-    CONF_DEFAULT_CONSIDER_UNAVAILABLE_BATTERY,
-    CONF_DEFAULT_CONSIDER_UNAVAILABLE_MAINS,
-    CONF_ENABLE_IDENTIFY_ON_JOIN,
     POWER_BATTERY_OR_UNKNOWN,
     POWER_MAINS_POWERED,
     UNKNOWN,
     UNKNOWN_MANUFACTURER,
     UNKNOWN_MODEL,
     ZHA_CLUSTER_HANDLER_CFG_DONE,
     ZHA_CLUSTER_HANDLER_MSG,
     ZHA_EVENT,
-    ZHA_OPTIONS,
 )
-from zha.application.helpers import async_get_zha_config_value, convert_to_zcl_values
+from zha.application.helpers import convert_to_zcl_values
 from zha.application.platforms import PlatformEntity, PlatformEntityInfo
 from zha.event import EventBase
 from zha.exceptions import ZHAException
 from zha.mixins import LogMixin
 from zha.zigbee.cluster_handlers import ClusterHandler, ZDOClusterHandler
 from zha.zigbee.endpoint import Endpoint
 
@@ -195,16 +188,14 @@
     routes: list[RouteInfo]
     endpoint_names: list[EndpointNameInfo]
 
 
 class Device(LogMixin, EventBase):
     """ZHA Zigbee device object."""
 
-    _ha_device_id: str
-
     def __init__(
         self,
         zigpy_device: zigpy.device.Device,
         _gateway: Gateway,
     ) -> None:
         """Initialize the gateway."""
         super().__init__()
@@ -219,38 +210,30 @@
         )
         self.quirk_id: str | None = getattr(self._zigpy_device, ATTR_QUIRK_ID, None)
         self._power_config_ch: ClusterHandler | None = None
         self._identify_ch: ClusterHandler | None = None
         self._basic_ch: ClusterHandler | None = None
         self._sw_build_id: int | None = None
 
+        device_options = _gateway.config.config.device_options
         if self.is_mains_powered:
-            self.consider_unavailable_time: int = async_get_zha_config_value(
-                self._gateway.config,
-                ZHA_OPTIONS,
-                CONF_CONSIDER_UNAVAILABLE_MAINS,
-                CONF_DEFAULT_CONSIDER_UNAVAILABLE_MAINS,
+            self.consider_unavailable_time: int = (
+                device_options.consider_unavailable_mains
             )
         else:
-            self.consider_unavailable_time = async_get_zha_config_value(
-                self._gateway.config,
-                ZHA_OPTIONS,
-                CONF_CONSIDER_UNAVAILABLE_BATTERY,
-                CONF_DEFAULT_CONSIDER_UNAVAILABLE_BATTERY,
-            )
+            self.consider_unavailable_time = device_options.consider_unavailable_battery
         self._available: bool = self.is_active_coordinator or (
             self.last_seen is not None
             and time.time() - self.last_seen < self.consider_unavailable_time
         )
         self._checkins_missed_count: int = 0
         self._on_network: bool = True
 
         self._platform_entities: dict[str, PlatformEntity] = {}
         self.semaphore: asyncio.Semaphore = asyncio.Semaphore(3)
-        self._tracked_tasks: list[asyncio.Task] = []
         self._zdo_handler: ZDOClusterHandler = ZDOClusterHandler(self)
         self.status: DeviceStatus = DeviceStatus.CREATED
 
         self._endpoints: dict[int, Endpoint] = {}
         for ep_id, endpoint in zigpy_device.endpoints.items():
             if ep_id != 0:
                 self._endpoints[ep_id] = Endpoint.new(endpoint, self)
@@ -492,15 +475,15 @@
         """Return the platform entities for this device."""
         return self._platform_entities
 
     def get_platform_entity(self, unique_id: str) -> PlatformEntity:
         """Get a platform entity by unique id."""
         entity = self._platform_entities.get(unique_id)
         if entity is None:
-            raise ValueError(f"Entity {unique_id} not found")
+            raise KeyError(f"Entity {unique_id} not found")
         return entity
 
     @classmethod
     def new(
         cls,
         zigpy_dev: zigpy.device.Device,
         gateway: Gateway,
@@ -697,19 +680,16 @@
                 for route in topology.routes[self.ieee]
             ],
             endpoint_names=names,
         )
 
     async def async_configure(self) -> None:
         """Configure the device."""
-        should_identify = async_get_zha_config_value(
-            self._gateway.config,
-            ZHA_OPTIONS,
-            CONF_ENABLE_IDENTIFY_ON_JOIN,
-            True,
+        should_identify = (
+            self.gateway.config.config.device_options.enable_identify_on_join
         )
         self.debug("started configuration")
         await self._zdo_handler.async_configure()
         self._zdo_handler.debug("'async_configure' stage succeeded")
         await asyncio.gather(
             *(endpoint.async_configure() for endpoint in self._endpoints.values())
         )
@@ -755,20 +735,14 @@
 
         self.debug("power source: %s", self.power_source)
         self.status = DeviceStatus.INITIALIZED
         self.debug("completed initialization")
 
     async def on_remove(self) -> None:
         """Cancel tasks this device owns."""
-        tasks = [t for t in self._tracked_tasks if not (t.done() or t.cancelled())]
-        for task in tasks:
-            self.debug("Cancelling task: %s", task)
-            task.cancel()
-        with suppress(asyncio.CancelledError):
-            await asyncio.gather(*tasks, return_exceptions=True)
         for platform_entity in self._platform_entities.values():
             await platform_entity.on_remove()
 
     def async_get_clusters(self) -> dict[int, dict[str, dict[int, Cluster]]]:
         """Get all clusters for this device."""
         return {
             ep_id: {
@@ -806,26 +780,21 @@
         clusters: dict[int, dict[str, dict[int, Cluster]]] = self.async_get_clusters()
         return clusters[endpoint_id][cluster_type][cluster_id]
 
     def async_get_cluster_attributes(
         self, endpoint_id, cluster_id, cluster_type=CLUSTER_TYPE_IN
     ):
         """Get zigbee attributes for specified cluster."""
-        cluster = self.async_get_cluster(endpoint_id, cluster_id, cluster_type)
-        if cluster is None:
-            return None
-        return cluster.attributes
+        return self.async_get_cluster(endpoint_id, cluster_id, cluster_type).attributes
 
     def async_get_cluster_commands(
         self, endpoint_id, cluster_id, cluster_type=CLUSTER_TYPE_IN
     ):
         """Get zigbee commands for specified cluster."""
         cluster = self.async_get_cluster(endpoint_id, cluster_id, cluster_type)
-        if cluster is None:
-            return None
         return {
             CLUSTER_COMMANDS_CLIENT: cluster.client_commands,
             CLUSTER_COMMANDS_SERVER: cluster.server_commands,
         }
 
     async def write_zigbee_attribute(
         self,
```

### Comparing `zha-0.0.7/zha/zigbee/endpoint.py` & `zha-0.0.8/zha/zigbee/endpoint.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha/zigbee/group.py` & `zha-0.0.8/zha/zigbee/group.py`

 * *Files identical despite different names*

### Comparing `zha-0.0.7/zha.egg-info/PKG-INFO` & `zha-0.0.8/zha.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library implementing ZHA for Home Assistant
 Author-email: "David F. Mulcahey" <david.mulcahey@icloud.com>
 License: GPL-3.0
 Project-URL: repository, https://github.com/zigpy/zha
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `zha-0.0.7/zha.egg-info/SOURCES.txt` & `zha-0.0.8/zha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 setup.py
 tests/test_alarm_control_panel.py
 tests/test_async_.py
 tests/test_binary_sensor.py
 tests/test_button.py
 tests/test_climate.py
 tests/test_cluster_handlers.py
-tests/test_color.py
 tests/test_cover.py
 tests/test_debouncer.py
 tests/test_device.py
 tests/test_device_tracker.py
 tests/test_discover.py
 tests/test_event.py
 tests/test_executor.py
```

